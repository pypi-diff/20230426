# Comparing `tmp/pdftoolkit-0.1.0.tar.gz` & `tmp/pdftoolkit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdftoolkit-0.1.0.tar", max compression
+gzip compressed data, was "pdftoolkit-0.2.1.tar", max compression
```

## Comparing `pdftoolkit-0.1.0.tar` & `pdftoolkit-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       34 2023-04-26 01:54:03.810278 pdftoolkit-0.1.0/pdftoolkit/__init__.py
--rw-r--r--   0        0        0     2039 2023-04-26 01:44:28.743298 pdftoolkit-0.1.0/pdftoolkit/PDFToolkit.py
--rw-r--r--   0        0        0      334 2023-04-26 01:53:31.147563 pdftoolkit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-26 01:49:24.127594 pdftoolkit-0.1.0/README.md
--rw-r--r--   0        0        0      300 1970-01-01 00:00:00.000000 pdftoolkit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       34 2023-04-26 01:54:03.810278 pdftoolkit-0.2.1/pdftoolkit/__init__.py
+-rw-r--r--   0        0        0     2290 2023-04-26 02:15:10.245665 pdftoolkit-0.2.1/pdftoolkit/PDFToolkit.py
+-rw-r--r--   0        0        0      355 2023-04-26 02:17:45.057082 pdftoolkit-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      103 2023-04-26 01:59:14.556493 pdftoolkit-0.2.1/README.md
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 pdftoolkit-0.2.1/PKG-INFO
```

### Comparing `pdftoolkit-0.1.0/pdftoolkit/PDFToolkit.py` & `pdftoolkit-0.2.1/pdftoolkit/PDFToolkit.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 from PyPDF2.errors import PdfReadError
 import os
 
 class PDFToolkit:
     def __init__(self):
         pass
 
-    def pdf2image(pdfPath, outputPath, imageFormat):
+    def pdf2image(pdfPath, outputPath, imageFormat,  imagename=None):
         """
         Converte um arquivo PDF em uma ou mais imagens no formato especificado e salva na pasta de saída.
 
         :param pdfPath: o caminho completo do arquivo PDF a ser convertido
         :param outputPath: o caminho completo da pasta onde as imagens convertidas serão salvas
         :param imageFormat: o formato das imagens de saída (por exemplo, 'png', 'jpeg', etc.)
+        :param imagename: o nome das imagens de saída (opcional)
         :return: nenhum
 
         Exemplo de uso:
         pdf_toolkit = PDFToolkit()
         pdf_toolkit.convert_pdf_to_images('/caminho/para/arquivo.pdf', '/caminho/para/pasta', 'jpeg')
 
         Esta função converte um arquivo PDF em uma ou mais imagens no formato especificado e salva na pasta de saída. O nome das imagens de saída é gerado automaticamente a partir do nome do arquivo PDF e do número da página. Se o arquivo PDF contém várias páginas, a função gera uma imagem para cada página. As imagens são salvas na pasta de saída com o nome no formato 'nome_do_arquivo_pdf_número_da_página.extensão'.
@@ -33,8 +34,11 @@
             except PdfReadError:
                 raise ValueError(f'O arquivo PDF {pdfPath} é inválido e não pode ser convertido.')
 
         # Converte o arquivo PDF em imagens
         fileName = os.path.splitext(os.path.basename(pdfPath))[0]
         pages = convert_from_path(pdfPath)
         for i, page in enumerate(pages):
-            page.save(os.path.join(outputPath, f'{fileName}_{i+1}.{imageFormat}'), f'{imageFormat}')
+            if imagename is not None:
+                page.save(os.path.join(outputPath, f'{imagename}_{i+1}.{imageFormat}'), f'{imageFormat}')
+            else:
+                page.save(os.path.join(outputPath, f'{fileName}_{i+1}.{imageFormat}'), f'{imageFormat}')
```

