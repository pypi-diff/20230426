# Comparing `tmp/overreact-1.1.0.tar.gz` & `tmp/overreact-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overreact-1.1.0.tar", max compression
+gzip compressed data, was "overreact-1.2.0.tar", max compression
```

## Comparing `overreact-1.1.0.tar` & `overreact-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1091 2021-11-03 17:50:30.000000 overreact-1.1.0/LICENSE
--rw-r--r--   0        0        0     7177 2023-01-04 22:50:48.820821 overreact-1.1.0/README.md
--rw-r--r--   0        0        0     3039 2023-01-04 22:50:48.820821 overreact-1.1.0/overreact/__init__.py
--rw-r--r--   0        0        0    36911 2023-01-04 22:44:00.477287 overreact-1.1.0/overreact/_cli.py
--rw-r--r--   0        0        0     4125 2023-01-04 22:44:00.469287 overreact-1.1.0/overreact/_constants.py
--rw-r--r--   0        0        0      962 2023-01-04 22:44:00.457287 overreact-1.1.0/overreact/_datasets.py
--rw-r--r--   0        0        0    15694 2023-01-04 22:44:00.461287 overreact-1.1.0/overreact/_misc.py
--rw-r--r--   0        0        0    29367 2023-01-04 22:44:00.477287 overreact-1.1.0/overreact/api.py
--rw-r--r--   0        0        0    64413 2023-01-04 22:44:00.485288 overreact-1.1.0/overreact/coords.py
--rw-r--r--   0        0        0    27226 2023-01-04 22:44:00.465288 overreact-1.1.0/overreact/core.py
--rw-r--r--   0        0        0    36044 2023-01-04 22:44:00.453287 overreact-1.1.0/overreact/io.py
--rw-r--r--   0        0        0    12472 2023-01-04 22:44:00.437287 overreact-1.1.0/overreact/rates.py
--rw-r--r--   0        0        0    22984 2023-01-04 23:01:10.256182 overreact-1.1.0/overreact/simulate.py
--rw-r--r--   0        0        0    30914 2023-01-04 22:44:00.409288 overreact-1.1.0/overreact/thermo/__init__.py
--rw-r--r--   0        0        0    31839 2023-01-04 22:44:00.417287 overreact-1.1.0/overreact/thermo/_gas.py
--rw-r--r--   0        0        0    10516 2023-01-04 22:44:00.401287 overreact-1.1.0/overreact/thermo/_solv.py
--rw-r--r--   0        0        0     8244 2023-01-04 22:44:00.405288 overreact-1.1.0/overreact/tunnel.py
--rw-r--r--   0        0        0     2537 2023-01-04 23:00:48.608201 overreact-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     8433 1970-01-01 00:00:00.000000 overreact-1.1.0/setup.py
--rw-r--r--   0        0        0     9186 1970-01-01 00:00:00.000000 overreact-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2021-11-03 17:50:30.000000 overreact-1.2.0/LICENSE
+-rw-r--r--   0        0        0     7177 2023-04-25 20:47:49.671926 overreact-1.2.0/README.md
+-rw-r--r--   0        0        0     3064 2023-04-25 20:06:11.911990 overreact-1.2.0/overreact/__init__.py
+-rw-r--r--   0        0        0    37574 2023-04-25 20:06:11.931991 overreact-1.2.0/overreact/_cli.py
+-rw-r--r--   0        0        0     4141 2023-04-25 20:06:11.911990 overreact-1.2.0/overreact/_constants.py
+-rw-r--r--   0        0        0     1189 2023-04-25 20:06:11.915990 overreact-1.2.0/overreact/_datasets.py
+-rw-r--r--   0        0        0    15743 2023-04-25 20:06:11.923991 overreact-1.2.0/overreact/_misc.py
+-rw-r--r--   0        0        0    29905 2023-04-25 20:06:11.927991 overreact-1.2.0/overreact/api.py
+-rw-r--r--   0        0        0    66022 2023-04-25 20:06:11.931991 overreact-1.2.0/overreact/coords.py
+-rw-r--r--   0        0        0    27491 2023-04-25 20:06:11.915990 overreact-1.2.0/overreact/core.py
+-rw-r--r--   0        0        0    36823 2023-04-25 20:06:11.931991 overreact-1.2.0/overreact/io.py
+-rw-r--r--   0        0        0    12633 2023-04-25 20:06:11.919990 overreact-1.2.0/overreact/rates.py
+-rw-r--r--   0        0        0    22645 2023-04-25 20:06:11.915990 overreact-1.2.0/overreact/simulate.py
+-rw-r--r--   0        0        0    31246 2023-04-25 20:06:11.923991 overreact-1.2.0/overreact/thermo/__init__.py
+-rw-r--r--   0        0        0    31990 2023-04-25 20:06:11.927991 overreact-1.2.0/overreact/thermo/_gas.py
+-rw-r--r--   0        0        0    10753 2023-04-25 20:06:11.919990 overreact-1.2.0/overreact/thermo/_solv.py
+-rw-r--r--   0        0        0     8350 2023-04-25 20:06:11.919990 overreact-1.2.0/overreact/tunnel.py
+-rw-r--r--   0        0        0     2566 2023-04-25 20:47:31.963717 overreact-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8433 1970-01-01 00:00:00.000000 overreact-1.2.0/setup.py
+-rw-r--r--   0        0        0     9190 1970-01-01 00:00:00.000000 overreact-1.2.0/PKG-INFO
```

### Comparing `overreact-1.1.0/LICENSE` & `overreact-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `overreact-1.1.0/README.md` & `overreact-1.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -161,22 +161,22 @@
   number        = {3},
   pages         = {209–217},
   doi           = {10.1002/jcc.26861},
   issn          = {1096-987x},
   url           = {http://dx.doi.org/10.1002/jcc.26861},
 }
 @software{overreact_software2021,
-  title         = {geem-lab/overreact: v1.1.0 \vert{} Zenodo},
+  title         = {geem-lab/overreact: v1.2.0 \vert{} Zenodo},
   author        = {Felipe S. S. Schneider and Let\'{\i}cia M. P. Madureira and  Giovanni F. Caramori},
   year          = {2023},
   month         = {Jan},
   publisher     = {Zenodo},
   doi           = {10.5281/zenodo.7504800},
   url           = {https://doi.org/10.5281/zenodo.7504800},
-  version       = {v1.1.0},
+  version       = {v1.2.0},
   howpublished  = {\url{https://github.com/geem-lab/overreact}},
 }
 ```
 
 ## License
 
 **overreact** is open-source, released under the permissive **MIT license**. See
```

#### html2text {}

```diff
@@ -47,18 +47,18 @@
 www.bibtex.org/) format: ```bibtex @article{overreact_paper2022, title =
 {Overreact, an in silico lab: Automative quantum chemical microkinetic
 simulations for complex chemical reactions}, author = {Schneider, Felipe S. S.
 and Caramori, Giovanni F.}, year = {2022}, month = {Apr}, journal = {Journal of
 Computational Chemistry}, publisher = {Wiley}, volume = {44}, number = {3},
 pages = {209â217}, doi = {10.1002/jcc.26861}, issn = {1096-987x}, url =
 {http://dx.doi.org/10.1002/jcc.26861}, } @software{overreact_software2021,
-title = {geem-lab/overreact: v1.1.0 \vert{} Zenodo}, author = {Felipe S. S.
+title = {geem-lab/overreact: v1.2.0 \vert{} Zenodo}, author = {Felipe S. S.
 Schneider and Let\'{\i}cia M. P. Madureira and Giovanni F. Caramori}, year =
 {2023}, month = {Jan}, publisher = {Zenodo}, doi = {10.5281/zenodo.7504800},
-url = {https://doi.org/10.5281/zenodo.7504800}, version = {v1.1.0},
+url = {https://doi.org/10.5281/zenodo.7504800}, version = {v1.2.0},
 howpublished = {\url{https://github.com/geem-lab/overreact}}, } ``` ## License
 **overreact** is open-source, released under the permissive **MIT license**.
 See [the LICENSE agreement](https://github.com/geem-lab/overreact/blob/main/
 LICENSE). ## Funding This project was developed at the [GEEM lab](https://geem-
 ufsc.org/) ([Federal University of Santa Catarina](https://en.ufsc.br/),
 Brazil), and was partially funded by the [Brazilian National Council for
 Scientific and Technological Development (CNPq)](https://cnpq.br/), grant
```

### Comparing `overreact-1.1.0/overreact/__init__.py` & `overreact-1.2.0/overreact/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python3  # noqa: EXE001
 
 """
 .. include:: ../README.md
 """  # noqa: D200, D400
 __docformat__ = "restructuredtext"
 
 import pkg_resources as _pkg_resources
@@ -86,13 +86,14 @@
   publisher     = {Zenodo},
   doi           = {ZENODO_DOI_PLACEHOLDER},
   url           = {https://doi.org/ZENODO_DOI_PLACEHOLDER},
   version       = {vVERSION_PLACEHOLDER},
   howpublished  = {\url{URL_REPO_PLACEHOLDER}},
 }
 """.replace(  # noqa: E501
-        "ZENODO_DOI_PLACEHOLDER", __zenodo_doi__
+        "ZENODO_DOI_PLACEHOLDER",
+        __zenodo_doi__,
     )
     .replace("DOI_PLACEHOLDER", __doi__)
     .replace("URL_REPO_PLACEHOLDER", __url_repo__)
     .replace("VERSION_PLACEHOLDER", __version__)
 )
```

### Comparing `overreact-1.1.0/overreact/_cli.py` & `overreact-1.2.0/overreact/_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python3  # noqa: EXE001
 
 """Command-line interface."""
 
 
 from __future__ import annotations
 
 import argparse
@@ -126,28 +126,28 @@
     ──────────────────────────────────────────────────────────────────────────────
     0   S -> S         No         8.17e+10      8.17e+10      8.17e+10     1.11
     <BLANKLINE>
     Only in the table above, all Gibbs free energies were biased by 0.0 J/mol.
     For half-equilibria, only ratios make sense: in simulations, equilibria will be
     adjusted to be faster than all other reactions.
     ────────────────────────────────────────────────────────────────────────────────
-    """  # noqa: E501
+    """
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,  # noqa: ANN101
         model,
         concentrations=None,
         savepath=None,
         plot=None,
         qrrho_descriptor="both",
         temperature=298.15,
         pressure=constants.atm,
         bias=0.0,
         tunneling="eckart",
-        method="LSODA",
+        method="RK23",
         max_time=1 * 60 * 60,
         rtol=1e-3,
         atol=1e-6,
         box_style=box.SIMPLE,
     ) -> None:
         """Initialize a Report object."""
         self.model = model
@@ -169,15 +169,15 @@
         self.tunneling = tunneling
         self.method = method
         self.max_time = max_time
         self.rtol = rtol
         self.atol = atol
         self.box_style = box_style
 
-    def __rich_console__(self, console, options):  # noqa: ANN101, ARG002, ANN204
+    def __rich_console__(self, console, options):  # noqa: ANN101, ANN204
         """
         Implement Rich Console protocol.
 
         This works by yielding from generators.
 
         Yields
         ------
@@ -195,26 +195,30 @@
 
         This is meant to be used from within `__rich_console__`.
 
         Yields
         ------
         renderable
         """
-        scheme = rx.core._check_scheme(self.model.scheme)
+        scheme = rx.core._check_scheme(self.model.scheme)  # noqa: SLF001
 
         raw_table = Table(
-            title="(read) reactions", box=self.box_style, show_header=False
+            title="(read) reactions",
+            box=self.box_style,
+            show_header=False,
         )
         raw_table.add_column(justify="left")
         for r in rx.core.unparse_reactions(scheme).split("\n"):
             raw_table.add_row(r)
         yield Panel(raw_table, expand=False)
 
         transition_states = rx.core.get_transition_states(
-            scheme.A, scheme.B, scheme.is_half_equilibrium
+            scheme.A,
+            scheme.B,
+            scheme.is_half_equilibrium,
         )
 
         parsed_table = Table(
             Column("no", justify="right"),
             Column("reactant(s)", justify="left"),
             Column("via‡", justify="left"),
             Column("product(s)", justify="left"),
@@ -247,16 +251,16 @@
             If at least one compound has undefined data.
         """
         undefined_compounds = []
         for name in self.model.compounds:
             if not self.model.compounds[name]:
                 undefined_compounds.append(name)
         if undefined_compounds:
-            raise ValueError(
-                f"undefined compounds: {', '.join(undefined_compounds)}"  # noqa: EM102
+            raise ValueError(  # noqa: TRY003
+                f"undefined compounds: {', '.join(undefined_compounds)}",  # noqa: EM102
             )  # noqa: RUF100
 
         logfiles_table = Table(
             Column("no", justify="right"),
             Column("compound", justify="left"),
             Column("path", justify="left"),
             title="logfiles",
@@ -278,20 +282,21 @@
                 path_text = Text(data.logfile)
                 path_text.highlight_regex(r"[^\/]+$", "bright_blue")
             logfiles_table.add_row(f"{i:d}", name, path_text)
 
             vibfreqs_text = None
             if data.vibfreqs is not None:
                 vibfreqs_text = Text(
-                    ", ".join([f"{vibfreq:+7.1f}" for vibfreq in data.vibfreqs[:3]])
+                    ", ".join([f"{vibfreq:+7.1f}" for vibfreq in data.vibfreqs[:3]]),
                 )
                 vibfreqs_text.highlight_regex(r"-\d+\.\d", "bright_yellow")
 
             point_group = coords.find_point_group(
-                atommasses=data.atommasses, atomcoords=data.atomcoords
+                atommasses=data.atommasses,
+                atomcoords=data.atomcoords,
             )
             compounds_table.add_row(
                 f"{i:d}",
                 name,
                 f"{data.energy / (constants.hartree * constants.N_A):17.12f}",
                 f"{data.mult}",
                 vibfreqs_text,
@@ -305,30 +310,36 @@
 
         This is meant to be used from within `__rich_console__`.
 
         Yields
         ------
         renderable
         """
-        scheme = rx.core._check_scheme(self.model.scheme)
+        scheme = rx.core._check_scheme(self.model.scheme)  # noqa: SLF001
 
         molecular_masses = np.array(
-            [np.sum(data.atommasses) for name, data in self.model.compounds.items()]
+            [np.sum(data.atommasses) for name, data in self.model.compounds.items()],
         )
         energies = np.array(
-            [data.energy for name, data in self.model.compounds.items()]
+            [data.energy for name, data in self.model.compounds.items()],
         )
         internal_energies = rx.get_internal_energies(
-            self.model.compounds, qrrho=self.qrrho, temperature=self.temperature
+            self.model.compounds,
+            qrrho=self.qrrho,
+            temperature=self.temperature,
         )
         enthalpies = rx.get_enthalpies(
-            self.model.compounds, qrrho=self.qrrho, temperature=self.temperature
+            self.model.compounds,
+            qrrho=self.qrrho,
+            temperature=self.temperature,
         )
         entropies = rx.get_entropies(
-            self.model.compounds, qrrho=self.qrrho, temperature=self.temperature
+            self.model.compounds,
+            qrrho=self.qrrho,
+            temperature=self.temperature,
         )
         freeenergies = enthalpies - self.temperature * entropies
         assert np.allclose(
             freeenergies,
             rx.get_freeenergies(
                 self.model.compounds,
                 qrrho=self.qrrho,
@@ -362,45 +373,54 @@
 
         delta_mass = rx.get_delta(scheme.A, molecular_masses)
         delta_energies = rx.get_delta(scheme.A, energies)
         delta_internal_energies = rx.get_delta(scheme.A, internal_energies)
         delta_enthalpies = rx.get_delta(scheme.A, enthalpies)
         # TODO(schneiderfelipe): log the contribution of reaction symmetry
         delta_entropies = rx.get_delta(scheme.A, entropies) + rx.get_reaction_entropies(
-            scheme.A, temperature=self.temperature, pressure=self.pressure
+            scheme.A,
+            temperature=self.temperature,
+            pressure=self.pressure,
         )
         delta_freeenergies = delta_enthalpies - self.temperature * delta_entropies
         assert np.allclose(
             delta_freeenergies,
             rx.get_delta(scheme.A, freeenergies)
             - self.temperature
             * rx.get_reaction_entropies(
-                scheme.A, temperature=self.temperature, pressure=self.pressure
+                scheme.A,
+                temperature=self.temperature,
+                pressure=self.pressure,
             ),
         ), "reaction free energies do not match reaction enthalpies and reaction entropies"  # noqa: E501
 
         delta_activation_mass = rx.get_delta(scheme.B, molecular_masses)
         delta_activation_energies = rx.get_delta(scheme.B, energies)
         delta_activation_internal_energies = rx.get_delta(scheme.B, internal_energies)
         delta_activation_enthalpies = rx.get_delta(scheme.B, enthalpies)
         # TODO(schneiderfelipe): log the contribution of reaction symmetry
         delta_activation_entropies = rx.get_delta(
-            scheme.B, entropies
+            scheme.B,
+            entropies,
         ) + rx.get_reaction_entropies(
-            scheme.B, temperature=self.temperature, pressure=self.pressure
+            scheme.B,
+            temperature=self.temperature,
+            pressure=self.pressure,
         )
         delta_activation_freeenergies = (
             delta_activation_enthalpies - self.temperature * delta_activation_entropies
         )
         assert np.allclose(
             delta_activation_freeenergies,
             rx.get_delta(scheme.B, freeenergies)
             - self.temperature
             * rx.get_reaction_entropies(
-                scheme.B, temperature=self.temperature, pressure=self.pressure
+                scheme.B,
+                temperature=self.temperature,
+                pressure=self.pressure,
             ),
         ), "activation free energies do not match activation enthalpies and activation entropies"  # noqa: E501
 
         circ_table = Table(
             Column("no", justify="right"),
             Column("reaction", justify="left"),
             Column("Δmass°\n〈amu〉", justify="center"),
@@ -469,15 +489,15 @@
                 ]
 
             circ_table.add_row(*circ_row)
             dagger_table.add_row(*dagger_row)
         yield circ_table
         yield dagger_table
 
-    def _yield_kinetics(self):  # noqa: ANN101, C901
+    def _yield_kinetics(self):  # noqa: ANN101, C901, PLR0912, PLR0915
         """Produce a renderables describing the kinetics of the system.
 
         This is meant to be used from within `__rich_console__`.
 
         Yields
         ------
         renderable
@@ -580,23 +600,25 @@
                 row[2] = "Yes"
                 row[-1] = None  # hide transmission coefficient
 
             kinetics_table.add_row(*row)
         yield kinetics_table
         yield Markdown(
             "Only in the table above, all Gibbs free energies were biased by "
-            f"{self.bias} J/mol."
+            f"{self.bias} J/mol.",
         )
         yield Markdown(
-            "For **half-equilibria**, only ratios make sense: in simulations, **equilibria will be adjusted to be faster than all other reactions**."  # noqa: E501
+            "For **half-equilibria**, only ratios make sense: in simulations, **equilibria will be adjusted to be faster than all other reactions**.",  # noqa: E501
         )
 
         if self.concentrations is not None and self.concentrations:
             scheme, k, y0 = _prepare_simulation(
-                self.model.scheme, k["M⁻ⁿ⁺¹·s⁻¹"], self.concentrations
+                self.model.scheme,
+                k["M⁻ⁿ⁺¹·s⁻¹"],
+                self.concentrations,
             )
 
             # TODO(schneiderfelipe): encapsulate everything in a function that depends
             # on the freeenergies as first parameter
             dydt = rx.get_dydt(scheme, k)
 
             y, r = rx.get_y(
@@ -626,16 +648,16 @@
                     f"{y(y.t_min)[i]:.3f}",
                     f"{y(y.t_max)[i]:.3f}",
                 )
             yield conc_table
 
             t_span = y.t_max - y.t_min
             active = ~np.isclose(
-                y(y.t_min + 0.01 * t_span * np.random.rand()),
-                y(y.t_max - 0.01 * t_span * np.random.rand()),
+                y(y.t_min + 0.01 * t_span * np.random.rand()),  # noqa: NPY002
+                y(y.t_max - 0.01 * t_span * np.random.rand()),  # noqa: NPY002
                 rtol=0.01,
             )
             if self.plot == "all" or not np.any(active):
                 active = np.array([True for _ in scheme.compounds])
 
             factor = y(y.t_max)[active].max()
             reference = y(y.t_max)[active] / factor
@@ -645,15 +667,17 @@
 
             # We plot until concentrations are within this value from the
             # final concentrations.
             alpha = 0.01
 
             t_max, i = y.t_max, 0
             while i < n_max and np.allclose(
-                y(t_max)[active] / factor, reference, atol=alpha
+                y(t_max)[active] / factor,
+                reference,
+                atol=alpha,
             ):
                 t_max = step * t_max
                 i += 1
 
             num = 100
             t = set(np.linspace(y.t_min, t_max, num=num))
             for i, name in enumerate(scheme.compounds):
@@ -664,15 +688,21 @@
                         method="bounded",
                     )
                     if y.t_min < res.x < t_max:
                         t.update(np.linspace(y.t_min, res.x, num=num // 2))
                         t.update(np.linspace(res.x, t_max, num=num // 2))
                         active[i] = True
 
-            t.update(np.geomspace(np.min([_t for _t in t if _t > 0.0]), t_max, num=num))
+            t.update(
+                np.geomspace(
+                    np.min([_t for _t in t if _t > 0.0]),  # noqa: PLR2004
+                    t_max,
+                    num=num,
+                ),
+            )
             t = np.array(sorted(t))
             if self.plot not in {"none", None}:
                 if self.plot not in {"all", "active"}:
                     name = self.plot
                     plt.plot(t, y(t)[scheme.compounds.index(name)], label=name, lw=3)
                 else:
                     for i, name in enumerate(scheme.compounds):
@@ -714,17 +744,17 @@
             quantity = quantity[1:]
         else:
             d = free_y0
 
         try:
             quantity = float(quantity)
         except (IndexError, ValueError):
-            raise ValueError(  # noqa: B904
+            raise ValueError(  # noqa: B904, TRY003, TRY200
                 "badly formatted concentrations: "  # noqa: EM102
-                f"'{' '.join(concentrations)}'"  # noqa: RUF100
+                f"'{' '.join(concentrations)}'",  # noqa: RUF100
             )
 
         d[name] = quantity
 
     # TODO(schneiderfelipe): log stuff related to get_fixed_scheme
     scheme, k = rx.get_fixed_scheme(scheme, k, fixed_y0)
 
@@ -766,15 +796,17 @@
         "concentrations",
         help="(optional) initial compound concentrations (in moles per liter) "
         "in the form 'name:quantity' (if present, a microkinetic simulation "
         "will be performed; more than one entry can be given)",
         nargs="*",
     )
     parser.add_argument(
-        "--version", action="version", version=f"%(prog)s {rx.__version__}"
+        "--version",
+        action="version",
+        version=f"%(prog)s {rx.__version__}",
     )
     parser.add_argument(
         "-v",
         "--verbose",
         help="increase output verbosity (can be given many times, each time "
         "the amount of logged data is increased)",
         action="count",
@@ -837,16 +869,16 @@
         type=float,
         default=constants.atm,
     )
     parser.add_argument(
         "--method",
         help="integrator used in solving the ODE system of the microkinetic "
         "simulation",
-        choices=["BDF", "Radau", "LSODA"],
-        default="LSODA",
+        choices=["RK23", "DOP853", "RK45", "LSODA", "BDF", "Radau"],
+        default="RK23",
     )
     parser.add_argument(
         "--max-time",
         help="maximum microkinetic simulation time (in s) allowed",
         type=float,
         default=1 * 60 * 60,
     )
@@ -911,30 +943,31 @@
 - Max. Time      = {args.max_time}
 - Rel. Tol.      = {args.rtol}
 - Abs. Tol.      = {args.atol}
 - Bias           = {bias_message}
 - Tunneling      = {args.tunneling}
 
 Parsing and calculating (this may take a while)…
-            """
+            """,
         ),
         justify="left",
     )
 
     logging.basicConfig(
-        level=levels[min(len(levels) - 1, args.verbose)], stream=sys.stdout
+        level=levels[min(len(levels) - 1, args.verbose)],
+        stream=sys.stdout,
     )
     for handler in logging.root.handlers:
         handler.setFormatter(rx.io.InterfaceFormatter("%(message)s"))
 
     model = rx.io.parse_model(args.path, force_compile=args.compile)
     report = Report(
         model,
         concentrations=args.concentrations,
-        savepath=f"{os.path.splitext(args.path)[0]}.csv",
+        savepath=f"{os.path.splitext(args.path)[0]}.csv",  # noqa: PTH122
         plot=args.plot,
         qrrho_descriptor=args.qrrho_descriptor,
         temperature=args.temperature,
         pressure=args.pressure,
         bias=args.bias,
         tunneling=args.tunneling,
         method=args.method,
```

### Comparing `overreact-1.1.0/overreact/_constants.py` & `overreact-1.2.0/overreact/_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python3  # noqa: EXE001
 
 """Module for storing constant data such as physical fundamental constants.
 
 Most of this data comes from `scipy.constants`.
 """
 
 import numpy as np
```

### Comparing `overreact-1.1.0/overreact/_datasets.py` & `overreact-1.2.0/overreact/_datasets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python3  # noqa: EXE001
 
 """Small toy datasets for tests and benchmark."""
 
 import os
 
 import overreact as rx
 
-data_path = os.path.normpath(os.path.join(os.path.dirname(__file__), "../data/"))
+data_path = os.path.normpath(
+    os.path.join(os.path.dirname(__file__), "../data/"),  # noqa: PTH118, PTH120
+)
 
 
 logfiles = {}
 for name in os.listdir(data_path):
-    walk_dir = os.path.join(data_path, name)
-    if os.path.isdir(walk_dir):
-        logfiles[name] = rx.io._LazyDict()
-        logfiles[name]._function = rx.io.read_logfile
+    walk_dir = os.path.join(data_path, name)  # noqa: PTH118
+    if os.path.isdir(walk_dir):  # noqa: PTH112
+        logfiles[name] = rx.io._LazyDict()  # noqa: SLF001
+        logfiles[name]._function = rx.io.read_logfile  # noqa: SLF001
         for root, _, files in os.walk(walk_dir):
             for filename in files:
                 if filename.endswith(".out"):
                     logfiles[name][
                         f"{filename[:-4]}@{os.path.relpath(root, walk_dir)}".replace(
-                            "@.", ""
+                            "@.",
+                            "",
                         )
-                    ] = os.path.join(root, filename)
+                    ] = os.path.join(  # noqa: PTH118
+                        root,
+                        filename,
+                    )
 
 
 if __name__ == "__main__":
     for name in logfiles:
         for compound in logfiles[name]:
             print(name, compound, logfiles[name][compound].logfile)  # noqa: T201
```

### Comparing `overreact-1.1.0/overreact/_misc.py` & `overreact-1.2.0/overreact/_misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python3  # noqa: EXE001
 
 """Miscellaneous functions that do not currently fit in other modules.
 
 Ideally, the functions here will be transferred to other modules in the future.
 """
 
 from functools import lru_cache as cache
@@ -514,15 +514,15 @@
     _check_package("thermo", _found_thermo, "solvents")
     # TODO(schneiderfelipe): return a named tuple with only the required data.
     # TODO(schneiderfelipe): support logging the retrieval of data.
     # TODO(schneiderfelipe): test returned parameters.
     return Chemical(identifier, temperature, pressure, *args, **kwargs)
 
 
-def broaden_spectrum(
+def broaden_spectrum(  # noqa: PLR0913
     x,
     x0,
     y0,
     distribution="gaussian",
     scale=1.0,
     fit_points=True,  # noqa: FBT002
     *args,  # noqa: ANN002
@@ -581,24 +581,28 @@
     elif distribution in {"lorentzian", "cauchy"}:
         distribution = cauchy
 
     s = np.sum(
         [
             yp
             * distribution.pdf(
-                x, xp, scale=scale, *args, **kwargs  # noqa: RUF004, B026
+                x,
+                xp,
+                scale=scale,
+                *args,  # noqa: B026
+                **kwargs,
             )  # noqa: RUF100
             for xp, yp in zip(x0, y0)
         ],
         axis=0,
     )
 
     if fit_points:
         s_max = np.max(s)
-        if s_max == 0.0:
+        if s_max == 0.0:  # noqa: PLR2004
             s_max = 1.0
         return s * np.max(y0) / s_max
     return s
 
 
 # https://stackoverflow.com/a/10016613
 def totuple(a):
@@ -618,15 +622,15 @@
     >>> totuple(array)
     ((2, 2), (2, -2))
     """
     # we don't touch some types, and this includes namedtuples
     if isinstance(a, (int, float, str, rx.Scheme)):
         return a
 
-    try:
+    try:  # noqa: SIM105
         a = a.tolist()
     except AttributeError:
         pass
 
     try:
         return tuple(totuple(i) for i in a)
     except TypeError:
@@ -696,28 +700,25 @@
 
     >>> x = halton(1500)
     >>> np.mean(x)  # estimate of the integral of x between 0 and 1
     0.50
     >>> np.mean(x**2)  # estimate of the integral of x**2 between 0 and 1
     0.33
     """
-    if dim is None:
-        actual_dim = 1
-    else:
-        actual_dim = dim
+    actual_dim = 1 if dim is None else dim
 
     res = np.array(
         [
             [_vdc(i, b) for i in range(jump, jump + num)]
             for b in _first_primes(actual_dim)
-        ]
+        ],
     )
 
     if cranley_patterson:
-        res = (res + np.random.rand(actual_dim, 1)) % 1.0
+        res = (res + np.random.rand(actual_dim, 1)) % 1.0  # noqa: NPY002
     if dim is None:
         return res.reshape((num,))
     return res.T
 
 
 def _first_primes(size):
     """Help haltonspace.
@@ -730,18 +731,15 @@
     [2, 3, 5, 7]
     >>> _first_primes(10)
     [2, 3, 5, 7, 11, 13, 17, 19, 23, 29]
     """
 
     def _is_prime(num):
         """Check if num is prime."""
-        for i in range(2, int(np.sqrt(num)) + 1):
-            if (num % i) == 0:
-                return False
-        return True
+        return all(num % i != 0 for i in range(2, int(np.sqrt(num)) + 1))
 
     primes = [2]
     p = 3
     while len(primes) < size:
         if _is_prime(p):
             primes.append(p)
         p += 2
```

### Comparing `overreact-1.1.0/overreact/api.py` & `overreact-1.2.0/overreact/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python3  # noqa: EXE001
 
 """
 This module contains the high-level application programming interface.
 
 If you intend to use **overreact** as a library in a project, you should
 probably start here.
 """  # noqa: D404
@@ -26,15 +26,15 @@
 
 import numpy as np
 from scipy.misc import derivative
 
 import overreact as rx
 from overreact import _constants as constants
 from overreact import coords, rates, tunnel
-from overreact.core import Scheme
+from overreact.core import Scheme  # noqa: TCH001
 
 logger = logging.getLogger(__name__)
 
 
 def get_internal_energies(
     compounds: dict,
     qrrho: bool = True,  # noqa: FBT001, FBT002
@@ -65,23 +65,24 @@
     >>> import overreact as rx
     >>> from overreact import _constants as constants
     >>> model = rx.parse_model("data/ethane/B97-3c/model.k")
     >>> internal_energies = get_internal_energies(model.compounds)
     >>> (internal_energies - internal_energies.min()) / constants.kcal
     array([0. , 2.20053981])
 
-    """  # noqa: E501
-    compounds = rx.io._check_compounds(compounds)
+    """
+    compounds = rx.io._check_compounds(compounds)  # noqa: SLF001
     internal_energies = []
     for name in compounds:
-        logger.info(f"calculate internal energy: {name}")
+        logger.info(f"calculate internal energy: {name}")  # noqa: G004
 
         # TODO(schneiderfelipe): inertia might benefit from caching
         moments, _, _ = coords.inertia(
-            compounds[name].atommasses, compounds[name].atomcoords
+            compounds[name].atommasses,
+            compounds[name].atomcoords,
         )
 
         internal_energy = rx.thermo.calc_internal_energy(
             energy=compounds[name].energy,
             degeneracy=compounds[name].mult,
             moments=moments,
             vibfreqs=compounds[name].vibfreqs,
@@ -130,38 +131,39 @@
     e.g., in the calculation of the Eckart tunneling coefficient, see
     `overreact.tunnel.eckart`). We can use this to calculate, for instance,
     the thermal contributions to the enthalpy:
 
     >>> zero_enthalpies = get_enthalpies(model.compounds, temperature=0)
     >>> (enthalpies - zero_enthalpies) / constants.kcal
     array([2.78, 2.50])
-    """  # noqa: E501
-    compounds = rx.io._check_compounds(compounds)
+    """
+    compounds = rx.io._check_compounds(compounds)  # noqa: SLF001
     enthalpies = []
     for name in compounds:
-        logger.info(f"calculate enthalpy: {name}")
+        logger.info(f"calculate enthalpy: {name}")  # noqa: G004
 
         # TODO(schneiderfelipe): inertia might benefit from caching
         moments, _, _ = coords.inertia(
-            compounds[name].atommasses, compounds[name].atomcoords
+            compounds[name].atommasses,
+            compounds[name].atomcoords,
         )
 
         enthalpy = rx.thermo.calc_enthalpy(
             energy=compounds[name].energy,
             degeneracy=compounds[name].mult,
             moments=moments,
             vibfreqs=compounds[name].vibfreqs,
             qrrho=qrrho,
             temperature=temperature,
         )
         enthalpies.append(enthalpy)
     return np.array(enthalpies)
 
 
-def get_entropies(
+def get_entropies(  # noqa: PLR0913
     compounds: dict,
     environment: Optional[str] = None,  # noqa: UP007
     method: str = "standard",
     qrrho: bool = True,  # noqa: FBT001, FBT002
     temperature: float = 298.15,
     pressure: float = constants.atm,
 ):
@@ -213,35 +215,37 @@
     array([1.4, 0. ])
 
     You can consider all compounds as solvated if you want:
 
     >>> sol_entropies = get_entropies(model.compounds, environment="solvent")
     >>> (sol_entropies - entropies) / constants.calorie
     array([-6.35360874, -6.35360874])
-    """  # noqa: E501
-    compounds = rx.io._check_compounds(compounds)
+    """
+    compounds = rx.io._check_compounds(compounds)  # noqa: SLF001
     entropies = []
     for name in compounds:
-        logger.info(f"calculate entropy: {name}")
+        logger.info(f"calculate entropy: {name}")  # noqa: G004
 
         if "point_group" in compounds[name]:
             point_group = compounds[name].point_group
         else:
             point_group = coords.find_point_group(
-                compounds[name].atommasses, compounds[name].atomcoords
+                compounds[name].atommasses,
+                compounds[name].atomcoords,
             )
         symmetry_number = coords.symmetry_number(point_group)
 
         # TODO(schneiderfelipe): inertia might benefit from caching
         moments, _, _ = coords.inertia(
-            compounds[name].atommasses, compounds[name].atomcoords
+            compounds[name].atommasses,
+            compounds[name].atomcoords,
         )
 
         if environment is None:
-            environment = rx.core._get_environment(name)
+            environment = rx.core._get_environment(name)  # noqa: SLF001
         entropy = rx.thermo.calc_entropy(
             atommasses=compounds[name].atommasses,
             atomcoords=compounds[name].atomcoords,
             energy=compounds[name].energy,
             degeneracy=compounds[name].mult,
             moments=moments,
             symmetry_number=symmetry_number,
@@ -264,15 +268,15 @@
             )
 
         entropies.append(entropy)
     return np.array(entropies)
 
 
 def _check_qrrho(
-    qrrho: Union[bool, tuple[bool, bool]]  # noqa: UP007
+    qrrho: Union[bool, tuple[bool, bool]],  # noqa: UP007
 ) -> tuple[bool, bool]:  # noqa: RUF100
     """Get options for QRRHO for both enthalpy and entropy.
 
     Parameters
     ----------
     qrrho : bool or tuple-like
         Apply both the quasi-rigid rotor harmonic oscillator (QRRHO)
@@ -297,26 +301,28 @@
     (True, True)
     >>> _check_qrrho(False)
     (False, False)
     >>> _check_qrrho((True, False))
     (True, False)
     >>> _check_qrrho((False, True))
     (False, True)
-    """  # noqa: E501
-    if qrrho is True:  # noqa: RET505
+    """
+    if qrrho is True:
         return True, True
-    elif qrrho is False:
+    elif qrrho is False:  # noqa: RET505
         return False, False
     elif isinstance(qrrho, tuple):
         return qrrho
     else:
-        raise ValueError(f"unrecognized QRRHO specification: {qrrho}")  # noqa: EM102
+        raise ValueError(  # noqa: TRY003
+            f"unrecognized QRRHO specification: {qrrho}",  # noqa: EM102
+        )
 
 
-def get_freeenergies(
+def get_freeenergies(  # noqa: PLR0913
     compounds: dict,
     bias: float = 0.0,
     environment: Optional[str] = None,  # noqa: UP007
     method: str = "standard",
     qrrho: Union[bool | tuple[bool, bool]] = True,  # noqa: FBT002, UP007
     temperature: float = 298.15,
     pressure: float = constants.atm,
@@ -384,32 +390,34 @@
 
     >>> get_freeenergies(model.compounds, bias=1.0) - freeenergies
     array([1., 1.])
     >>> get_freeenergies(model.compounds, bias=-1.0) - freeenergies
     array([-1., -1.])
     >>> get_freeenergies(model.compounds, bias=[1.0, -1.0]) - freeenergies
     array([ 1., -1.])
-    """  # noqa: E501
+    """
     qrrho_enthalpy, qrrho_entropy = _check_qrrho(qrrho)
     enthalpies = get_enthalpies(
-        compounds, qrrho=qrrho_enthalpy, temperature=temperature
+        compounds,
+        qrrho=qrrho_enthalpy,
+        temperature=temperature,
     )
     entropies = get_entropies(
         compounds,
         environment=environment,
         method=method,
         qrrho=qrrho_entropy,
         temperature=temperature,
         pressure=pressure,
     )
     # TODO(schneiderfelipe): log the contribution of bias
     return enthalpies - temperature * entropies + np.asarray(bias)
 
 
-def get_k(
+def get_k(  # noqa: PLR0913
     scheme: Scheme,
     compounds: Optional[dict] = None,  # noqa: UP007
     bias: float = 0.0,
     tunneling: str = "eckart",
     qrrho: Union[bool | tuple[bool, bool]] = True,  # noqa: FBT002, UP007
     scale: str = "l mol-1 s-1",
     temperature: float = 298.15,
@@ -530,17 +538,17 @@
     array([5.14e-13])
     >>> get_k(model.scheme, model.compounds,
     ...       bias=np.array([0.0, 0.0, -1.4, 0.0, 0.0]) * constants.kcal,
     ...       temperature=300.0, scale="cm3 particle-1 s-1")
     array([1.1e-12])
     """  # noqa: E501
     qrrho_enthalpy, qrrho_entropy = _check_qrrho(qrrho)
-    scheme = rx.core._check_scheme(scheme)
+    scheme = rx.core._check_scheme(scheme)  # noqa: SLF001
     if compounds is not None:
-        compounds = rx.io._check_compounds(compounds)
+        compounds = rx.io._check_compounds(compounds)  # noqa: SLF001
     if delta_freeenergies is None:
         assert compounds is not None, "compounds could not be inferred"
         freeenergies = get_freeenergies(
             compounds,
             bias=bias,
             qrrho=(qrrho_enthalpy, qrrho_entropy),
             # NOTE(schneiderfelipe): ensure we get rate constants in M-1 s-1.
@@ -549,17 +557,20 @@
             environment="solvent",
             temperature=temperature,
             pressure=pressure,
         )
 
         # TODO(schneiderfelipe): log the contribution of reaction symmetry
         delta_freeenergies = rx.get_delta(
-            scheme.B, freeenergies
+            scheme.B,
+            freeenergies,
         ) - temperature * rx.get_reaction_entropies(
-            scheme.B, temperature=temperature, pressure=pressure
+            scheme.B,
+            temperature=temperature,
+            pressure=pressure,
         )
 
     if molecularity is None:
         molecularity = rx.thermo.get_molecularity(scheme.A)
 
     # NOTE(schneiderfelipe): passing molecularity here to rates.eyring messes up
     # rate constant units (by a factor of M-1 s-1 to atm-1 s-1), so we leave it as is.
@@ -574,18 +585,18 @@
     i = 0
     while i < len(scheme.is_half_equilibrium):
         if scheme.is_half_equilibrium[i]:
             pair = k[i : i + 2]
             _K = pair[0] / pair[1]  # noqa: N806
 
             denom = pair.min()
-            if denom == 0.0:
+            if denom == 0.0:  # noqa: PLR2004
                 logger.warning(
                     "found half-equilibrium reaction with zero rate constant: "
-                    "skipping equilibrium normalization"
+                    "skipping equilibrium normalization",
                 )
                 denom = 1.0
 
             k[i : i + 2] = pair / denom
             assert np.isclose(_K, k[i] / k[i + 1]), (
                 f"reaction rate constants {k[i]} and {k[i + 1]} for "
                 "equilibria could not be made to match the expected "
@@ -593,16 +604,16 @@
             )
 
             # loop over pairs of equilibria
             i += 1
         i += 1
 
     logger.info(
-        "(classical) reaction rate constants: "
-        f"{', '.join([f'{v:7.3g}' for v in k])} atm⁻ⁿ⁺¹·s⁻¹"
+        "(classical) reaction rate constants: "  # noqa: G004
+        f"{', '.join([f'{v:7.3g}' for v in k])} atm⁻ⁿ⁺¹·s⁻¹",
     )
     if tunneling not in {"none", None}:
         if compounds is not None:
             kappa = get_kappa(
                 scheme,
                 compounds,
                 method=tunneling,
@@ -611,19 +622,19 @@
             )
             k *= kappa
         else:
             # TODO(schneiderfelipe): when get_kappa accept deltas, this will
             # be probably unnecessary.
             logger.warning(
                 "assuming unitary tunneling coefficients due to incomplete "
-                "compound data"
+                "compound data",
             )
         logger.info(
-            "(tunneling) reaction rate constants: "
-            f"{', '.join([f'{v:7.3g}' for v in k])} atm⁻ⁿ⁺¹·s⁻¹"
+            "(tunneling) reaction rate constants: "  # noqa: G004
+            f"{', '.join([f'{v:7.3g}' for v in k])} atm⁻ⁿ⁺¹·s⁻¹",
         )
 
     # TODO(schneiderfelipe): ensure diffusional limit for reactions in
     # solvation using Collins-Kimball theory. This includes half-equilibria.
     return rates.convert_rate_constant(
         k,
         new_scale=scale,
@@ -700,30 +711,31 @@
 
     You can calculate each piece of the reaction rate constant by hand,
     if you want. Just make sure that you don't calculate the tunneling
     coefficient twice:
 
     >>> kappa * get_k(model.scheme, model.compounds, tunneling=None)
     array([8.e+10])
-    """  # noqa: E501
-    scheme = rx.core._check_scheme(scheme)
-    compounds = rx.io._check_compounds(compounds)
+    """
+    scheme = rx.core._check_scheme(scheme)  # noqa: SLF001
+    compounds = rx.io._check_compounds(compounds)  # noqa: SLF001
 
     if method == "eckart":
         # NOTE(schneiderfelipe): We need electronic energies + ZPE here, so we
         # get smaller transmission coefficients.
         energies = get_enthalpies(compounds, qrrho=qrrho, temperature=0.0)
         delta_forward = rx.get_delta(scheme.B, energies)  # B - A
         delta_backward = delta_forward - rx.get_delta(
-            scheme.A, energies
+            scheme.A,
+            energies,
         )  # B - C == B - A - (C - A)
 
     kappas = []
     for i, ts in enumerate(
-        rx.get_transition_states(scheme.A, scheme.B, scheme.is_half_equilibrium)
+        rx.get_transition_states(scheme.A, scheme.B, scheme.is_half_equilibrium),
     ):
         if ts is None:
             kappas.append(1.0)
         else:
             transition_state = scheme.compounds[ts]
             vibfreq = compounds[transition_state].vibfreqs[0]
 
@@ -734,41 +746,45 @@
                         kappa = tunnel.eckart(
                             vibfreq,
                             delta_forward[i],
                             delta_backward[i],
                             temperature=temperature,
                         )
                     except RuntimeWarning as e:
-                        logger.warning(f"using Wigner tunneling correction: {e}")
+                        logger.warning(
+                            f"using Wigner tunneling correction: {e}",  # noqa: G004
+                        )
                         kappa = tunnel.wigner(vibfreq, temperature=temperature)
             elif method == "wigner":
                 kappa = tunnel.wigner(vibfreq, temperature=temperature)
             elif method in {"none", None}:
                 kappa = 1.0
             else:
-                raise ValueError(f"unavailable method: '{method}'")  # noqa: EM102
+                raise ValueError(  # noqa: TRY003
+                    f"unavailable method: '{method}'",  # noqa: EM102
+                )
 
             kappas.append(kappa)
 
     # TODO(schneiderfelipe): is this correct? shouldn't we correct shapes
     # somewhere else?
     vec_kappas = np.asarray(kappas).flatten()
     logger.info(
-        "(quantum) tunneling coefficients: "
-        f"{', '.join([f'{kappa:7.3g}' for kappa in vec_kappas])}"
+        "(quantum) tunneling coefficients: "  # noqa: G004
+        f"{', '.join([f'{kappa:7.3g}' for kappa in vec_kappas])}",
     )
     return vec_kappas
 
 
-def get_drc(
+def get_drc(  # noqa: PLR0913
     scheme,
     compounds,
     y0,
     t_span=None,
-    method="LSODA",
+    method="RK23",
     qrrho=True,  # noqa: FBT002
     scale="l mol-1 s-1",
     temperature=298.15,
     dx=1.5e3,  # joules
     order=3,
 ):
     """Calculate the degree of rate control for a single compound.
```

### Comparing `overreact-1.1.0/overreact/coords.py` & `overreact-1.2.0/overreact/coords.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python3  # noqa: EXE001
 
 """Module dedicated to classifying molecules into point groups."""
 
 
 # TODO: add types to this module
 from __future__ import annotations
 
@@ -21,15 +21,15 @@
 import overreact as rx
 from overreact import _constants as constants
 
 logger = logging.getLogger(__name__)
 
 
 # TODO(schneiderfelipe): alpha should depend on temperature?
-def get_molecular_volume(
+def get_molecular_volume(  # noqa: PLR0913
     atomnos,
     atomcoords,
     full_output=False,  # noqa: FBT002
     environment="water",
     method="garza",
     temperature=298.15,
     pressure=constants.atm,
@@ -132,55 +132,57 @@
     box_volume = np.prod(v2 - v1)
     n = int(num * box_volume)
 
     vdw_volumes = []
     if full_output and method == "izato":
         cav_volumes = []
     for _ in range(trials):
-        points = rx._misc.halton(n, 3)
+        points = rx._misc.halton(n, 3)  # noqa: SLF001
         points = v1 + points * (v2 - v1)
         tree = KDTree(points)
 
         within_vdw = set()
         if full_output and method == "izato":
             within_cav = set()
         for i, atomcoord in enumerate(atomcoords):
             within_vdw.update(tree.query_ball_point(atomcoord, vdw_radii[i]))
             if full_output and method == "izato":
                 within_cav.update(
-                    tree.query_ball_point(atomcoord, alpha * vdw_radii[i])
+                    tree.query_ball_point(atomcoord, alpha * vdw_radii[i]),
                 )
 
         vdw_volumes.append((len(within_vdw) / n) * box_volume)
         if full_output and method == "izato":
             cav_volumes.append((len(within_cav) / n) * box_volume)
 
     vdw_volume = np.mean(vdw_volumes)
     vdw_err = np.std(vdw_volumes)
-    logger.info(f"van der Waals volume = {vdw_volume} ± {vdw_err} Å³")
+    logger.info(f"van der Waals volume = {vdw_volume} ± {vdw_err} Å³")  # noqa: G004
     if full_output:
-        if method == "izato":  # noqa: RET505
+        if method == "izato":
             cav_volume = np.mean(cav_volumes)
             cav_err = np.std(cav_volumes)
-            logger.debug(f"Izato cavity volume = {cav_volume} ± {cav_err} Å³")
+            logger.debug(
+                f"Izato cavity volume = {cav_volume} ± {cav_err} Å³",  # noqa: G004
+            )
             return (vdw_volume, cav_volume, max(vdw_err, cav_err))
-        elif method == "garza":
+        elif method == "garza":  # noqa: RET505
             # TODO(schneiderfelipe): test for the following solvents: water,
             # pentane, hexane, heptane and octane.
 
             cav_volume = _garza(
                 vdw_volume,
                 environment,
                 temperature=temperature,
                 pressure=pressure,
             )
-            logger.debug(f"Garza cavity volume = {cav_volume} Å³")
+            logger.debug(f"Garza cavity volume = {cav_volume} Å³")  # noqa: G004
             return (vdw_volume, cav_volume, vdw_err)
         else:
-            raise ValueError(f"unavailable method: '{method}'")  # noqa: EM102
+            raise ValueError(f"unavailable method: '{method}'")  # noqa: EM102, TRY003
     return vdw_volume
 
 
 def _garza(
     vdw_volume,
     environment="water",
     full_output=False,  # noqa: FBT002
@@ -233,26 +235,26 @@
     >>> _garza(10.0, full_output=True, environment="benzene")
     (243., 3.29, 0.499372648682062)
     >>> _garza(100.0, environment="benzene")
     665.
     >>> _garza(100.0, full_output=True, environment="benzene")
     (665., 1.0, 1.07586575757374)
     """
-    solvent = rx._misc._get_chemical(environment, temperature, pressure)
+    solvent = rx._misc._get_chemical(environment, temperature, pressure)  # noqa: SLF001
 
     # TODO(schneiderfelipe): things to do:
     # 1. check correctness of this function,
     # 2. check it is called correctly everywhere,
     # 3. create a complete abstraction of the solvent/molecular properties:
 
     solvent_volume = solvent.Van_der_Waals_volume / (
         constants.angstrom**3 * constants.N_A
     )
     r_free = np.cbrt(
-        solvent.Vm / (constants.angstrom**3 * constants.N_A) - solvent_volume
+        solvent.Vm / (constants.angstrom**3 * constants.N_A) - solvent_volume,
     )
     r_M = np.cbrt(vdw_volume)  # noqa: N806
 
     cav_volume = (r_M + r_free) ** 3
     if not full_output:
         return cav_volume
     r_S = np.cbrt(solvent_volume)  # noqa: N806
@@ -312,15 +314,15 @@
     12
     >>> symmetry_number("D6") == symmetry_number("D6d")
     True
     >>> symmetry_number("S6")
     3
     >>> symmetry_number("T")
     12
-    """  # noqa: E501
+    """
     point_group = point_group.strip().lower()
 
     if point_group in {"c1", "ci", "cs", "c∞v", "k", "r3"}:
         symmetry_number = 1
     elif point_group in {"c2", "c2v", "c2h", "d∞h", "s4"}:
         symmetry_number = 2
     elif point_group in {"c4", "c4v", "c4h", "d2", "d2d", "d2h", "s8", "vh"}:
@@ -357,27 +359,30 @@
         "d30h",
         "s120",
         "ih",
     }:
         symmetry_number = 60
     else:
         pieces = re.match(
-            r"(?P<letter>[^\s]+)(?P<number>\d+)(?P<type>[^\s]+)?", point_group
+            r"(?P<letter>[^\s]+)(?P<number>\d+)(?P<type>[^\s]+)?",
+            point_group,
         ).groupdict()
 
         if pieces["letter"] == "c":
             symmetry_number = int(pieces["number"])
         elif pieces["letter"] == "d":
             symmetry_number = 2 * int(pieces["number"])
         elif pieces["letter"] == "s":
             symmetry_number = int(pieces["number"]) // 2
         else:
-            raise ValueError(f"unknown point group: '{point_group}'")  # noqa: EM102
+            raise ValueError(  # noqa: TRY003
+                f"unknown point group: '{point_group}'",  # noqa: EM102
+            )
 
-    logger.info(f"symmetry number = {symmetry_number}")
+    logger.info(f"symmetry number = {symmetry_number}")  # noqa: G004
     return symmetry_number
 
 
 def find_point_group(atommasses, atomcoords, proper_axes=None, rtol=0.0, atol=1.0e-2):
     """Determine point group of structure.
 
     Parameters
@@ -415,32 +420,37 @@
     ...                                     [0, 0, 0],
     ...                                     [1, 1, 0]])
     'D4h'
 
     """
     if len(atommasses) == 1:  # atom
         point_group = "K"
-    elif len(atommasses) == 2:  # diatomic molecule
-        if atommasses[0] == atommasses[1]:
-            point_group = "D∞h"
-        else:
-            point_group = "C∞v"
+    elif len(atommasses) == 2:  # diatomic molecule  # noqa: PLR2004
+        point_group = "D∞h" if atommasses[0] == atommasses[1] else "C∞v"
     else:
         groups = _equivalent_atoms(atommasses, atomcoords)
         moments, axes, atomcoords = inertia(atommasses, atomcoords)
         rotor_class = _classify_rotor(moments)
 
         if rotor_class[1] == "linear":
             point_group = _find_point_group_linear(
-                atomcoords, groups, rtol=rtol, atol=atol
+                atomcoords,
+                groups,
+                rtol=rtol,
+                atol=atol,
             )
         else:
             if proper_axes is None:
                 proper_axes = _get_proper_axes(
-                    atomcoords, groups, axes, rotor_class, rtol=rtol, atol=atol
+                    atomcoords,
+                    groups,
+                    axes,
+                    rotor_class,
+                    rtol=rtol,
+                    atol=atol,
                 )
 
             if rotor_class[0] == "asymmetric" or not proper_axes:
                 point_group = _find_point_group_asymmetric(
                     atomcoords,
                     groups,
                     axes,
@@ -466,32 +476,32 @@
                     axes,
                     rotor_class,
                     proper_axes,
                     rtol=rtol,
                     atol=atol,
                 )
 
-    logger.info(f"point group = {point_group}")
+    logger.info(f"point group = {point_group}")  # noqa: G004
     return point_group
 
 
 def _find_point_group_linear(atomcoords, groups, rtol=0.0, atol=1.0e-2):
     """Find point group for linear rotors.
 
     Point groups searched for are: D∞h, C∞v.
 
     See find_point_group for information on parameters and return values.
     """
-    if _has_inversion_center(atomcoords, groups, rtol=rtol, atol=atol):  # noqa: RET505
+    if _has_inversion_center(atomcoords, groups, rtol=rtol, atol=atol):
         return "D∞h"
-    else:
+    else:  # noqa: RET505
         return "C∞v"
 
 
-def _find_point_group_spheric(
+def _find_point_group_spheric(  # noqa: PLR0913
     atomcoords,
     groups,
     axes,
     rotor_class,
     proper_axes=None,
     rtol=0.0,
     atol=1.0e-2,
@@ -504,34 +514,39 @@
     See find_point_group for information on parameters and return values.
     """
     if not _has_inversion_center(atomcoords, groups, rtol=rtol, atol=atol):
         return "Td"
 
     if proper_axes is None:
         proper_axes = _get_proper_axes(
-            atomcoords, groups, axes, rotor_class, rtol=rtol, atol=atol
+            atomcoords,
+            groups,
+            axes,
+            rotor_class,
+            rtol=rtol,
+            atol=atol,
         )
 
     for n, _ in proper_axes:
-        if n == 5:  # noqa: RET505
+        if n == 5:  # noqa: PLR2004
             return "Ih"
-        elif n < 5:
+        elif n < 5:  # noqa: PLR2004, RET505
             break
     return "Oh"
 
     # see https://www.chem.uci.edu/~lawm/9-28.pdf for more about high
     # symmetry groups
     # see too
     # http://web.mit.edu/5.03/www/readings/point_groups/point_groups.pdf
 
     # the employed workflow is loosely inspired by some articles:
     # 1. doi:10.1016/0097-8485(76)80004-6
 
 
-def _find_point_group_asymmetric(
+def _find_point_group_asymmetric(  # noqa: PLR0913
     atomcoords,
     groups,
     axes,
     rotor_class,
     proper_axes=None,
     rtol=0.0,
     atol=1.0e-2,
@@ -541,40 +556,51 @@
     Point groups searched for here are: C1, Ci, Cs.
     Point groups delegated are: Cn, Cnh, Cnv, Dn, Dnh, Dnd, Sn.
 
     See find_point_group for information on parameters and return values.
     """
     if proper_axes is None:
         proper_axes = _get_proper_axes(
-            atomcoords, groups, axes, rotor_class, rtol=rtol, atol=atol
+            atomcoords,
+            groups,
+            axes,
+            rotor_class,
+            rtol=rtol,
+            atol=atol,
         )
 
-    if proper_axes:  # noqa: RET505
+    if proper_axes:
         return _find_point_group_symmetric(
             atomcoords,
             groups,
             axes,
             rotor_class,
             proper_axes,
             rtol=rtol,
             atol=atol,
         )
-    elif rotor_class[1] in {
+    elif rotor_class[1] in {  # noqa: RET505
         "regular planar",
         "irregular planar",
     } or _get_mirror_planes(
-        atomcoords, groups, axes, rotor_class, proper_axes, rtol=rtol, atol=atol
+        atomcoords,
+        groups,
+        axes,
+        rotor_class,
+        proper_axes,
+        rtol=rtol,
+        atol=atol,
     ):
         return "Cs"
     elif _has_inversion_center(atomcoords, groups, rtol=rtol, atol=atol):
         return "Ci"
     return "C1"
 
 
-def _find_point_group_symmetric(
+def _find_point_group_symmetric(  # noqa: PLR0913
     atomcoords,
     groups,
     axes,
     rotor_class,
     proper_axes=None,
     rtol=0.0,
     atol=1.0e-2,
@@ -583,43 +609,54 @@
 
     Point groups delegated are: Cn, Cnh, Cnv, Dn, Dnh, Dnd, Sn.
 
     See find_point_group for information on parameters and return values.
     """
     if proper_axes is None:
         proper_axes = _get_proper_axes(
-            atomcoords, groups, axes, rotor_class, rtol=rtol, atol=atol
+            atomcoords,
+            groups,
+            axes,
+            rotor_class,
+            rtol=rtol,
+            atol=atol,
         )
     n_principal = proper_axes[0][0]
 
     count_twofold = 0
     for n, _ in proper_axes:
-        if n == 2:
+        if n == 2:  # noqa: PLR2004
             count_twofold += 1
         if n_principal == count_twofold:
             return _find_point_group_symmetric_dihedral(
                 atomcoords,
                 groups,
                 axes,
                 rotor_class,
                 proper_axes,
                 rtol=rtol,
                 atol=atol,
             )
-        if n < 2:
+        if n < 2:  # noqa: PLR2004
             break
     return _find_point_group_symmetric_nondihedral(
-        atomcoords, groups, axes, rotor_class, proper_axes, rtol=rtol, atol=atol
+        atomcoords,
+        groups,
+        axes,
+        rotor_class,
+        proper_axes,
+        rtol=rtol,
+        atol=atol,
     )
 
     # the employed workflow is loosely inspired by some articles:
     # 1. doi:10.1016/0097-8485(76)80004-6
 
 
-def _find_point_group_symmetric_dihedral(
+def _find_point_group_symmetric_dihedral(  # noqa: PLR0913
     atomcoords,
     groups,
     axes,
     rotor_class,
     proper_axes=None,
     rtol=0.0,
     atol=1.0e-2,
@@ -628,30 +665,43 @@
 
     Point groups searched for are: Dn, Dnh, Dnd.
 
     See find_point_group for information on parameters and return values.
     """
     if proper_axes is None:
         proper_axes = _get_proper_axes(
-            atomcoords, groups, axes, rotor_class, rtol=rtol, atol=atol
+            atomcoords,
+            groups,
+            axes,
+            rotor_class,
+            rtol=rtol,
+            atol=atol,
         )
     mirror_axes = _get_mirror_planes(
-        atomcoords, groups, axes, rotor_class, proper_axes, rtol=rtol, atol=atol
+        atomcoords,
+        groups,
+        axes,
+        rotor_class,
+        proper_axes,
+        rtol=rtol,
+        atol=atol,
     )
 
     if mirror_axes:
-        if mirror_axes[0][0] == "h":  # noqa: RET505
+        if mirror_axes[0][0] == "h":
             return f"D{proper_axes[0][0]}h"
-        elif len([v for c, v in mirror_axes if c == "v"]) == proper_axes[0][0]:
+        elif (  # noqa: RET505
+            len([v for c, v in mirror_axes if c == "v"]) == proper_axes[0][0]
+        ):  # noqa: RET505, RUF100
             # all vertical mirror planes are dihedral for Dnd point groups
             return f"D{proper_axes[0][0]}d"
     return f"D{proper_axes[0][0]}"
 
 
-def _find_point_group_symmetric_nondihedral(
+def _find_point_group_symmetric_nondihedral(  # noqa: PLR0913
     atomcoords,
     groups,
     axes,
     rotor_class,
     proper_axes=None,
     rtol=0.0,
     atol=1.0e-2,
@@ -660,35 +710,54 @@
 
     Point groups searched for are: Cn, Cnh, Cnv, Sn.
 
     See find_point_group for information on parameters and return values.
     """
     if proper_axes is None:
         proper_axes = _get_proper_axes(
-            atomcoords, groups, axes, rotor_class, rtol=rtol, atol=atol
+            atomcoords,
+            groups,
+            axes,
+            rotor_class,
+            rtol=rtol,
+            atol=atol,
         )
     mirror_axes = _get_mirror_planes(
-        atomcoords, groups, axes, rotor_class, proper_axes, rtol=rtol, atol=atol
+        atomcoords,
+        groups,
+        axes,
+        rotor_class,
+        proper_axes,
+        rtol=rtol,
+        atol=atol,
     )
 
     if mirror_axes:
-        if mirror_axes[0][0] == "h":  # noqa: RET505
+        if mirror_axes[0][0] == "h":
             return f"C{proper_axes[0][0]}h"
-        elif len([v for c, v in mirror_axes if c == "v"]) == proper_axes[0][0]:
+        elif (  # noqa: RET505
+            len([v for c, v in mirror_axes if c == "v"]) == proper_axes[0][0]
+        ):  # noqa: RET505, RUF100
             return f"C{proper_axes[0][0]}v"
 
     improper_axes = _get_improper_axes(
-        atomcoords, groups, axes, rotor_class, proper_axes, rtol=rtol, atol=atol
+        atomcoords,
+        groups,
+        axes,
+        rotor_class,
+        proper_axes,
+        rtol=rtol,
+        atol=atol,
     )
     if improper_axes:
         return f"S{improper_axes[0][0]}"
     return f"C{proper_axes[0][0]}"
 
 
-def _update_proper_axes(
+def _update_proper_axes(  # noqa: PLR0913
     ax,
     axes,  # found axes
     atomcoords,
     groups,
     orders,
     rtol,
     atol,
@@ -725,16 +794,22 @@
         ):
             axes.append((order, tuple(ax)))
             return axes, order
 
     return axes, None
 
 
-def _get_proper_axes(  # noqa: C901
-    atomcoords, groups, axes, rotor_class, rtol=0.0, atol=1.0e-2, slack=0.735
+def _get_proper_axes(  # noqa: C901, PLR0912, PLR0913
+    atomcoords,
+    groups,
+    axes,
+    rotor_class,
+    rtol=0.0,
+    atol=1.0e-2,
+    slack=0.735,
 ):
     """Get proper symmetry axes and their orders.
 
     Parameters
     ----------
     atomcoords : array-like
         Atomic coordinates centered at the center of mass.
@@ -838,15 +913,15 @@
                 groups=groups,
                 orders=orders,
                 rtol=rtol,
                 atol=atol,
                 nondeg_axes=nondeg_axes,
                 normalize=True,
             )
-            if rotor_class[0] == "spheric" and order == 5:
+            if rotor_class[0] == "spheric" and order == 5:  # noqa: PLR2004
                 return sorted(found_axes, reverse=True)
 
             for b in group[:i]:
                 midpoint_ax = atomcoords[a] + atomcoords[b]
                 found_axes, order = _update_proper_axes(
                     midpoint_ax,
                     found_axes,
@@ -854,34 +929,34 @@
                     groups=groups,
                     orders=orders,
                     rtol=rtol,
                     atol=atol,
                     nondeg_axes=nondeg_axes,
                     normalize=True,
                 )
-                if rotor_class[0] == "spheric" and order == 5:
+                if rotor_class[0] == "spheric" and order == 5:  # noqa: PLR2004
                     return sorted(found_axes, reverse=True)
 
     if rotor_class[0] == "spheric":
-        twofold_axes = [ax for o, ax in found_axes if o == 2]
+        twofold_axes = [ax for o, ax in found_axes if o == 2]  # noqa: PLR2004
         for i, ax_a in enumerate(twofold_axes):
             for ax_b in twofold_axes[:i]:
                 ax = np.cross(ax_a, ax_b)
                 found_axes, order = _update_proper_axes(
                     ax,
                     found_axes,
                     atomcoords=atomcoords,
                     groups=groups,
                     orders=orders,
                     rtol=rtol,
                     atol=atol,
                     nondeg_axes=nondeg_axes,
                     normalize=True,
                 )
-                if order == 5:
+                if order == 5:  # noqa: PLR2004
                     return sorted(found_axes, reverse=True)
 
     return sorted(found_axes, reverse=True)
 
 
 def _guess_orders(groups, rotor_class):
     """Guess possible group orders based on groups.
@@ -918,15 +993,15 @@
     """
     max_order = len(groups[-1])
     if rotor_class[0] == "spheric":
         max_order = min(max_order, 5)
     return range(2, max_order + 1)
 
 
-def _update_improper_axes(
+def _update_improper_axes(  # noqa: PLR0913
     n,
     ax,
     axes,
     atomcoords,
     groups,
     rtol,
     atol,
@@ -954,15 +1029,15 @@
         ):
             axes.append((order, tuple(ax)))
             break
 
     return axes
 
 
-def _get_improper_axes(
+def _get_improper_axes(  # noqa: PLR0913
     atomcoords,
     groups,
     axes,
     rotor_class,
     proper_axes=None,
     rtol=0.0,
     atol=1.0e-2,
@@ -1012,15 +1087,20 @@
         return []
 
     axes = np.asarray(axes)
     atomcoords = np.asarray(atomcoords)
 
     if proper_axes is None:
         proper_axes = _get_proper_axes(
-            atomcoords, groups, axes, rotor_class, rtol=rtol, atol=atol
+            atomcoords,
+            groups,
+            axes,
+            rotor_class,
+            rtol=rtol,
+            atol=atol,
         )
 
     found_axes = []
     for n, ax in proper_axes:
         found_axes = _update_improper_axes(
             n,
             ax,
@@ -1029,15 +1109,15 @@
             groups=groups,
             rtol=rtol,
             atol=atol,
         )
     return sorted(found_axes, reverse=True)
 
 
-def _update_mirror_axes(
+def _update_mirror_axes(  # noqa: PLR0913
     ax,
     axes,  # found axes
     atomcoords,
     groups,
     rtol,
     atol,
     proper_axes,
@@ -1060,15 +1140,18 @@
     if not all(
         np.isclose(ax @ v, 0.0, rtol=rtol, atol=atol) for v in nondeg_axes
     ) or any(np.isclose(np.abs(ax @ v), 1.0, rtol=rtol, atol=atol) for c, v in axes):
         return axes
 
     if all(
         _is_symmetric(
-            atomcoords[group], _operation("sigma", axis=ax), rtol=rtol, atol=atol
+            atomcoords[group],
+            _operation("sigma", axis=ax),
+            rtol=rtol,
+            atol=atol,
         )
         for group in groups[::-1]
     ):
         class_ = ""
         if any(
             np.isclose(np.abs(ax @ v), 1.0, rtol=rtol, atol=atol)
             for n, v in proper_axes
@@ -1082,15 +1165,15 @@
         ):
             class_ = "v"
         axes.append((class_, tuple(ax)))
 
     return axes
 
 
-def _get_mirror_planes(  # noqa: C901
+def _get_mirror_planes(  # noqa: C901, PLR0913
     atomcoords,
     groups,
     axes,
     rotor_class,
     proper_axes=None,
     rtol=0.0,
     atol=1.0e-2,
@@ -1154,23 +1237,28 @@
         return []
 
     axes = np.asarray(axes)
     atomcoords = np.asarray(atomcoords)
 
     if proper_axes is None:
         proper_axes = _get_proper_axes(
-            atomcoords, groups, axes, rotor_class, rtol=rtol, atol=atol
+            atomcoords,
+            groups,
+            axes,
+            rotor_class,
+            rtol=rtol,
+            atol=atol,
         )
 
     def _kf(x):
         """Order function for returned list."""
         c, v = x
-        if c:  # noqa: RET505
+        if c:
             return -ord(c), v
-        else:
+        else:  # noqa: RET505
             return 0, v
 
     found_axes = []
     nondeg_axes = []
     if rotor_class[0] == "symmetric prolate":
         nondeg_axes = [axes[:, 0]]
         found_axes = _update_mirror_axes(
@@ -1392,34 +1480,37 @@
     array([[-1., 0.,  0.],
            [ 0., 0., -1.],
            [ 0., 1.,  0.]])
     """
     if axis is None:
         axis = np.array([0, 0, 1])
 
-    if name == "i":  # noqa: RET505
+    if name == "i":
         return -np.eye(3)
-    elif name == "e":
+    if name == "e":
         return np.eye(3)
-    elif name in {"c", "σ", "sigma", "s"}:  # noqa: RUF001
+
+    if name in {"c", "σ", "sigma", "s"}:  # noqa: RUF001
         # normalize axis
         axis = np.asarray(axis)
         axis = axis / np.linalg.norm(axis)
 
         if name in {"c", "s"}:
             rotation = Rotation.from_rotvec(2.0 * np.pi * axis / order).as_matrix()
         if name in {"σ", "sigma", "s"}:  # noqa: RUF001
             reflection = np.eye(3) - 2.0 * np.outer(axis, axis)
+
         if name == "c":
             return rotation
-        elif name in {"σ", "sigma"}:  # noqa: RUF001
+        if name in {"σ", "sigma"}:  # noqa: RUF001
             return reflection
-        elif name == "s":
+        if name == "s":
             return rotation @ reflection
-    raise ValueError(f"unknown operation: '{name}'")  # noqa: EM102
+
+    raise ValueError(f"unknown operation: '{name}'")  # noqa: EM102, TRY003
 
 
 def _classify_rotor(moments, rtol=0.0, atol=1.0e-2, slack=0.870):
     """Classify rotors based on moments of inertia.
 
     See doi:10.1002/jcc.23493.
 
@@ -1494,26 +1585,38 @@
 
     if np.isclose(moments[2], 0.0, rtol=inner_slack * rtol, atol=inner_slack * atol):
         return "spheric", "atomic"
     moments = np.asarray(moments) / moments[2]
 
     # basic tests for tops
     is_oblate = np.isclose(
-        moments[0], moments[1], rtol=inner_slack * rtol, atol=inner_slack * atol
+        moments[0],
+        moments[1],
+        rtol=inner_slack * rtol,
+        atol=inner_slack * atol,
     )
     is_spheric = np.isclose(
-        moments[0], moments[2], rtol=inner_slack * rtol, atol=inner_slack * atol
+        moments[0],
+        moments[2],
+        rtol=inner_slack * rtol,
+        atol=inner_slack * atol,
     )
     is_prolate = np.isclose(
-        moments[1], moments[2], rtol=inner_slack * rtol, atol=inner_slack * atol
+        moments[1],
+        moments[2],
+        rtol=inner_slack * rtol,
+        atol=inner_slack * atol,
     )
 
     # basic tests for shapes
     fits_line = np.isclose(
-        moments[0], 0.0, rtol=inner_slack * rtol, atol=inner_slack * atol
+        moments[0],
+        0.0,
+        rtol=inner_slack * rtol,
+        atol=inner_slack * atol,
     )
     fits_plane = np.isclose(moments[0] + moments[1], moments[2], rtol=rtol, atol=atol)
 
     is_spheric = is_spheric and is_oblate and is_prolate
     if is_spheric:
         top = "spheric"
     elif is_oblate:
@@ -1523,18 +1626,15 @@
     else:
         top = "asymmetric"
 
     fits_line = fits_line and is_prolate
     if fits_line:
         shape = "linear"
     elif fits_plane:
-        if is_oblate:
-            shape = "regular planar"
-        else:
-            shape = "irregular planar"
+        shape = "regular planar" if is_oblate else "irregular planar"
     else:
         shape = "nonplanar"
 
     return top, shape
 
 
 def gyradius(atommasses, atomcoords, method="iupac"):
@@ -1575,22 +1675,22 @@
     >>> gyradius(np.ones_like(data.atommasses), data.atomcoords, method="mean")
     0.6833818299241241
     >>> gyradius(data.atommasses, data.atomcoords, method="mean")
     0.7637734749747612
     """
     com = np.average(atomcoords, axis=0, weights=atommasses)
     atomcoords = atomcoords - com
-    if method == "iupac":  # noqa: RET505
+    if method == "iupac":
         return np.sqrt(
-            np.average(np.diag(atomcoords @ atomcoords.T), weights=atommasses)
+            np.average(np.diag(atomcoords @ atomcoords.T), weights=atommasses),
         )
-    elif method == "mean":
+    elif method == "mean":  # noqa: RET505
         return np.sqrt(np.mean(np.diag(atomcoords @ atomcoords.T)))
     else:
-        raise ValueError(f"unavailable method: '{method}'")  # noqa: EM102
+        raise ValueError(f"unavailable method: '{method}'")  # noqa: EM102, TRY003
 
 
 def inertia(atommasses, atomcoords, align=True):  # noqa: FBT002
     r"""Calculate primary moments and axes from the inertia tensor.
 
     Parameters
     ----------
@@ -1652,20 +1752,20 @@
     i_zz = np.sum(squared_w_coords[:, 0] + squared_w_coords[:, 1])
 
     i_xy = -np.sum(w_coords[:, 0] * w_coords[:, 1])
     i_xz = -np.sum(w_coords[:, 0] * w_coords[:, 2])
     i_yz = -np.sum(w_coords[:, 1] * w_coords[:, 2])
 
     inertia_tensor = np.array(
-        [[i_xx, i_xy, i_xz], [i_xy, i_yy, i_yz], [i_xz, i_yz, i_zz]]
+        [[i_xx, i_xy, i_xz], [i_xy, i_yy, i_yz], [i_xz, i_yz, i_zz]],
     )
     moments, axes = np.linalg.eigh(inertia_tensor)
     if align:
         return inertia(atommasses, atomcoords @ axes, align=False)
-    logger.debug(f"moments = {moments} amu·Å²")
+    logger.debug(f"moments = {moments} amu·Å²")  # noqa: G004
     return moments, axes, atomcoords
 
 
 # TODO(schneiderfelipe): this needs rework, see
 # https://chemistry.stackexchange.com/questions/74639/how-to-calculate-wavenumbers-of-normal-modes-from-the-eigenvalues-of-the-cartesi/74923#74923
 # Ideally, the same Eckart transformation that make this work will also work
 # in calc_vibfreqs, so one thing leads to the other.
@@ -1786,15 +1886,15 @@
 
     eigenvalues = np.linalg.eigvals(hessian)
 
     # TODO(schneiderfelipe): the following probably misses some linear
     # molecules and transition states.
     eigenvalues = np.real(eigenvalues[eigenvalues > 0])[::-1]
     nu = np.sqrt(
-        eigenvalues * constants.hartree / (constants.atomic_mass * constants.bohr**2)
+        eigenvalues * constants.hartree / (constants.atomic_mass * constants.bohr**2),
     ) / (2.0 * np.pi)
     return nu * constants.centi / constants.c
 
 
 # TODO(schneiderfelipe): ensure this is correct
 # https://chemistry.stackexchange.com/questions/74639/how-to-calculate-wavenumbers-of-normal-modes-from-the-eigenvalues-of-the-cartesi/74923#74923
 def eckart_transform(atommasses, atomcoords):
@@ -1862,52 +1962,56 @@
     moments, axes, atomcoords = inertia(atommasses, atomcoords, align=False)
 
     x = np.block(
         [
             np.ones(natom)[:, np.newaxis],
             np.zeros(natom)[:, np.newaxis],
             np.zeros(natom)[:, np.newaxis],
-        ]
+        ],
     )
     y = np.block(
         [
             np.zeros(natom)[:, np.newaxis],
             np.ones(natom)[:, np.newaxis],
             np.zeros(natom)[:, np.newaxis],
-        ]
+        ],
     )
     z = np.block(
         [
             np.zeros(natom)[:, np.newaxis],
             np.zeros(natom)[:, np.newaxis],
             np.ones(natom)[:, np.newaxis],
-        ]
+        ],
     )
     x *= np.sqrt(atommasses[:, np.newaxis])
     y *= np.sqrt(atommasses[:, np.newaxis])
     z *= np.sqrt(atommasses[:, np.newaxis])
 
     D_trans = np.block(  # noqa: N806
-        [x.reshape(1, dof).T, y.reshape(1, dof).T, z.reshape(1, dof).T]
+        [x.reshape(1, dof).T, y.reshape(1, dof).T, z.reshape(1, dof).T],
     )  # noqa: RUF100
     D_rot = np.array(  # noqa: N806
         [
             np.cross((atomcoords @ axes)[i], axes[:, j]) / np.sqrt(atommasses[i])
             for i in range(natom)
             for j in range(3)
-        ]
+        ],
     )
     D = np.block([D_trans, D_rot])  # noqa: N806
     return np.linalg.qr(D, mode="complete")[0]
 
 
 # NOTE(schneiderfelipe): thresh was found to be reasonable
 # when greater than or equal to 0.106.
 def _equivalent_atoms(  # noqa: C901
-    atommasses, atomcoords, method="cluster", thresh=0.106, plot=False  # noqa: FBT002
+    atommasses,
+    atomcoords,
+    method="cluster",
+    thresh=0.106,
+    plot=False,  # noqa: FBT002
 ):
     """Generate groups of symmetry equivalent atoms.
 
     Parameters
     ----------
     atommasses : array-like
         Atomic masses in atomic mass units (amu).
@@ -1959,17 +2063,17 @@
     ... )
     >>> for indices in _equivalent_atoms(atommasses, atomcoords):
     ...     indices
     [0]
     [1, 2, 3]
 
     """
-    if len(atommasses) == 1:  # atom  # noqa: RET505
+    if len(atommasses) == 1:  # atom
         return [[0]]
-    elif len(atommasses) == 2:  # diatomic molecule
+    elif len(atommasses) == 2:  # diatomic molecule  # noqa: PLR2004, RET505
         if atommasses[0] == atommasses[1]:
             return [[0, 1]]
         return [[0], [1]]
 
     groups = []
 
     def _update_groups_with_condition(condition, groups):
@@ -2004,16 +2108,17 @@
             plt.ylabel("sigma")
             plt.show()
 
         for mass in np.unique(atommasses):
             mass_condition = atommasses == mass
             for cluster in np.unique(clusters[mass_condition]):
                 groups = _update_groups_with_condition(
-                    mass_condition & (clusters == cluster), groups
+                    mass_condition & (clusters == cluster),
+                    groups,
                 )
     elif method == "atommass":
         for mass in np.unique(atommasses):
             groups = _update_groups_with_condition(atommasses == mass, groups)
     else:
-        raise ValueError(f"unavailable method: '{method}'")  # noqa: EM102
+        raise ValueError(f"unavailable method: '{method}'")  # noqa: EM102, TRY003
 
     return sorted(groups, key=len)
```

### Comparing `overreact-1.1.0/overreact/core.py` & `overreact-1.2.0/overreact/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python3  # noqa: EXE001
 
 """Module dedicated to parsing and modeling of chemical reaction networks."""
 
 
 __all__ = ["Scheme", "parse_reactions"]
 
 
@@ -245,24 +245,27 @@
     ...                      (0.0,)),
     ...                   B=((-1.0,),
     ...                      (1.0,))))
     'S -> E‡ -> S'
     """
     scheme = _check_scheme(scheme)
     transition_states = get_transition_states(
-        scheme.A, scheme.B, scheme.is_half_equilibrium
+        scheme.A,
+        scheme.B,
+        scheme.is_half_equilibrium,
     )
     lines = []
     i = 0
     while i < len(scheme.reactions):
         if transition_states[i] is not None:
             lines.append(
                 scheme.reactions[i].replace(
-                    "->", f"-> {scheme.compounds[transition_states[i]]} ->"
-                )
+                    "->",
+                    f"-> {scheme.compounds[transition_states[i]]} ->",
+                ),
             )
         elif scheme.is_half_equilibrium[i]:
             lines.append(scheme.reactions[i].replace("->", "<=>"))
             i += 1  # avoid backward reaction, which comes next
         else:
             lines.append(scheme.reactions[i])
         i += 1
@@ -337,15 +340,15 @@
 
     environment = token["environment"][1:-1].lower()
     if environment in {"l", "liquid"}:
         environment = name
 
     if environment in _abbr_environment:
         environment = _abbr_environment[environment]
-    return environment  # noqa: RET504
+    return environment
 
 
 def is_transition_state(name):
     """Check whether a name specifies a transition state.
 
     Parameters
     ----------
@@ -389,18 +392,15 @@
     >>> is_transition_state("A~(w)")
     False
     >>> is_transition_state("TS(w)")
     False
     >>> is_transition_state("TS~(w)")
     False
     """
-    for marker in {"‡", "#"}:
-        if marker in name:
-            return True
-    return False
+    return any(marker in name for marker in {"‡", "#"})
 
 
 def parse_reactions(text: Union[str, Sequence[str]]) -> Scheme:  # noqa: C901
     """
     Parse a kinetic model as a chemical reaction scheme.
 
     This is an essential part of the parsing process.
@@ -591,15 +591,16 @@
     In any case, it's not clear how a reaction barrier be defined in such a
     case. If you have a use case, don't hesitate to
     [open an issue](https://github.com/geem-lab/overreact/issues/), we'll be
     happy to hear from you.
     """
     compounds: dict[str, int] = {}
     reactions: dict[
-        tuple[str, str, bool, str], tuple[tuple[tuple[int, str], ...], bool]
+        tuple[str, str, bool, str],
+        tuple[tuple[tuple[int, str], ...], bool],
     ] = {}
     A = []  # coefficients between reactants and products  # noqa: N806
     B = []  # coefficients between reactants and transition states  # noqa: N806
 
     def _add_reaction(reactants, products, is_half_equilibrium, transition):
         """Local helper function with side-effects."""
         # TODO(schneiderfelipe): what if reaction is defined, then redefined
@@ -657,50 +658,55 @@
 
         # TODO(schneiderfelipe): what if a transition state is used in an
         # equilibrium?
 
         # it's assumed that if a transition shows up,
         #   1. it's the only compound in its side of the reaction, and
         #   2. its coefficient equals one
-        if is_transition_state(reactants[-1][-1]):  # noqa: RET507
+        if is_transition_state(reactants[-1][-1]):
             for before_reactants in before_transitions.get(reactants, []):
                 _add_reaction(
-                    before_reactants, products, is_half_equilibrium, reactants
+                    before_reactants,
+                    products,
+                    is_half_equilibrium,
+                    reactants,
                 )
 
             if reactants in after_transitions:
                 after_transitions[reactants].append(products)
             else:
                 after_transitions[reactants] = [products]
             continue
-        elif is_transition_state(products[-1][-1]):
+        elif is_transition_state(products[-1][-1]):  # noqa: RET507
             for after_products in after_transitions.get(products, []):
                 _add_reaction(reactants, after_products, is_half_equilibrium, products)
 
             if products in before_transitions:
                 before_transitions[products].append(reactants)
             else:
                 before_transitions[products] = [reactants]
             continue
 
         _add_reaction(reactants, products, is_half_equilibrium, None)
 
     return Scheme(
         compounds=tuple(compounds),
         reactions=tuple(_unparse_reactions(reactions)),
-        is_half_equilibrium=rx._misc.totuple([reaction[2] for reaction in reactions]),
-        A=rx._misc.totuple(
+        is_half_equilibrium=rx._misc.totuple(  # noqa: SLF001
+            [reaction[2] for reaction in reactions],
+        ),
+        A=rx._misc.totuple(  # noqa: SLF001
             np.block(
-                [[vector, np.zeros(len(compounds) - len(vector))] for vector in A]
-            ).T
+                [[vector, np.zeros(len(compounds) - len(vector))] for vector in A],
+            ).T,
         ),
-        B=rx._misc.totuple(
+        B=rx._misc.totuple(  # noqa: SLF001
             np.block(
-                [[vector, np.zeros(len(compounds) - len(vector))] for vector in B]
-            ).T
+                [[vector, np.zeros(len(compounds) - len(vector))] for vector in B],
+            ).T,
         ),
     )
 
 
 def _parse_reactions(text):
     r"""Parse reactions.
 
@@ -742,26 +748,28 @@
 
     """
     try:
         lines = text.split("\n")
     except AttributeError:
         lines = text
     for line in lines:
-        line = line.split("//")[0].strip()
+        line = line.split("//")[0].strip()  # noqa: PLW2901
         if not line:
             continue
 
         pieces = re.split(r"\s*(->|<=>|<-)\s*", line)
         for reactants, arrow, products in zip(
-            pieces[:-2:2], pieces[1:-1:2], pieces[2::2]
+            pieces[:-2:2],
+            pieces[1:-1:2],
+            pieces[2::2],
         ):
             if arrow == "<-":
-                reactants, products, arrow = products, reactants, "->"
-            reactants = tuple(_parse_side(reactants))
-            products = tuple(_parse_side(products))
+                reactants, products, arrow = products, reactants, "->"  # noqa: PLW2901
+            reactants = tuple(_parse_side(reactants))  # noqa: PLW2901
+            products = tuple(_parse_side(products))  # noqa: PLW2901
 
             if arrow == "<=>":
                 yield reactants, products, True
                 yield products, reactants, True
             else:
                 yield reactants, products, False
 
@@ -821,16 +829,17 @@
     other:
 
     >>> _unparse_side(_parse_side("   2     *A*1*    +  40B1  +  chlorophyll"))
     '2 *A*1* + 40 B1 + chlorophyll'
 
     """
     for token in re.split(r"\s+\+\s+", side):
-        token = re.match(
-            r"\s*(?P<coefficient>\d+)?\s*(?P<compound>[^\s]+)\s*", token
+        token = re.match(  # noqa: PLW2901
+            r"\s*(?P<coefficient>\d+)?\s*(?P<compound>[^\s]+)\s*",
+            token,
         ).groupdict(1)
         yield int(token["coefficient"]), token["compound"]
 
 
 def _unparse_side(unside):
     """Return string representation of a left/right hand side of a reaction.
```

### Comparing `overreact-1.1.0/overreact/io.py` & `overreact-1.2.0/overreact/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python3  # noqa: EXE001
 
 """Basic I/O operations (such as reading source **input files**)."""
 
 
 __all__ = ["parse_model"]
 
 
@@ -91,31 +91,33 @@
     True
     >>> model_from_source = parse_model("data/ethane/B97-3c/model")
     >>> model_from_source == model
     True
     """  # noqa: E501
     if not path.endswith((".k", ".jk")):
         path = f"{path}.jk"
-        logger.warning(f"assuming `.jk` file in {path}")
-    name, _ = os.path.splitext(path)
+        logger.warning(f"assuming `.jk` file in {path}")  # noqa: G004
+    name, _ = os.path.splitext(path)  # noqa: PTH122
 
     path_jk = f"{name}.jk"
-    if not force_compile and os.path.isfile(path_jk):
-        logger.info(f"parsing `.jk` file in {path_jk}")
+    if not force_compile and os.path.isfile(path_jk):  # noqa: PTH113
+        logger.info(f"parsing `.jk` file in {path_jk}")  # noqa: G004
         return _parse_model(path_jk)
 
     path_k = f"{name}.k"
-    logger.info(f"parsing `.k` file in {path_k}")
-    if not os.path.isfile(path_k):
+    logger.info(f"parsing `.k` file in {path_k}")  # noqa: G004
+    if not os.path.isfile(path_k):  # noqa: PTH113
         # TODO: add a nice error message here and everywhere?
-        raise FileNotFoundError(f"no `.k` file found in {path_k}")  # noqa: EM102
+        raise FileNotFoundError(  # noqa: TRY003
+            f"no `.k` file found in {path_k}",  # noqa: EM102
+        )
 
     model = _parse_source(path_k)
-    with open(path_jk, "w") as f:
-        logger.info(f"writing `.jk` file in {path_jk}")
+    with open(path_jk, "w") as f:  # noqa: PTH123
+        logger.info(f"writing `.jk` file in {path_jk}")  # noqa: G004
         f.write(_unparse_model(model))
 
     return model
 
 
 def _parse_model(file_or_path):
     """Parse a model input file (also known as a `.jk` file).
@@ -166,24 +168,24 @@
      'vibdisps': (((-6.7e-05, 2.3e-05, 3.4e-05),
                    ...,
                    (0.133315, 0.086028, 0.35746)))}
     """
     try:
         model = json.load(file_or_path)
     except AttributeError:
-        with open(file_or_path) as stream:
+        with open(file_or_path) as stream:  # noqa: PTH123
             model = json.load(stream)
 
     if "scheme" in model:
         model["scheme"] = rx.parse_reactions(model["scheme"])
 
     return dotdict(model)
 
 
-def _parse_source(file_path_or_str):  # noqa: C901
+def _parse_source(file_path_or_str):
     """Parse a source input file (also known as a `.k` file).
 
     A source input file contains all the information needed to create a model input file
     (also known as a `.jk` file).
 
     Parameters
     ----------
@@ -229,34 +231,31 @@
     True
     """
     name = None
     sections = defaultdict(list)
 
     path = ("",)
     try:
-        with open(file_path_or_str) as stream:
+        with open(file_path_or_str) as stream:  # noqa: PTH123
             lines = stream.readlines()
-        dirname = os.path.dirname(file_path_or_str)
+        dirname = os.path.dirname(file_path_or_str)  # noqa: PTH120
         if dirname not in path:
-            path = path + (dirname,)
+            path = (*path, dirname)
     except OSError:
         lines = file_path_or_str.split("\n")
     except TypeError:
         lines = file_path_or_str
 
     for line in lines:
-        line = line.split("//")[0].strip()
+        line = line.split("//")[0].strip()  # noqa: PLW2901
         if not line:
             continue
 
         if line[0] == "$":
-            if line[1:] == "end":
-                name = None
-            else:
-                name = line[1:]
+            name = None if line[1:] == "end" else line[1:]
         elif name is not None:
             sections[name].append(line)
 
     if "scheme" in sections:
         sections["scheme"] = rx.parse_reactions(sections["scheme"])
     if "compounds" in sections:
         sections["compounds"] = parse_compounds(
@@ -352,15 +351,16 @@
         source += "$end\n"
     if "compounds" in model:
         source += "$compounds\n"
         for compound in model.compounds:
             source += f" {compound}:\n"
             for key in model.compounds[compound]:
                 inline_json = json.dumps(
-                    model.compounds[compound][key], ensure_ascii=False
+                    model.compounds[compound][key],
+                    ensure_ascii=False,
                 )
                 source += f"  {key}={inline_json}\n"
         source += "$end\n"
     return source
 
 
 def _unparse_model(model):
@@ -436,15 +436,15 @@
     """
     for name in compounds:
         if isinstance(compounds[name], str):
             compounds[name] = read_logfile(compounds[name])
     return dict(compounds)
 
 
-def parse_compounds(text, path=("",), select=None):  # noqa: C901
+def parse_compounds(text, path=("",), select=None):  # noqa: C901, PLR0912
     """Parse a set of compounds.
 
     Parameters
     ----------
     text : str, sequence of str or dict-like
         Compound descriptions or sequence of lines of it.
     path : sequence of str, optional
@@ -529,15 +529,15 @@
         lines = text.split("\n")
     except AttributeError:
         lines = text
     name = None
     compounds = defaultdict(dict)
     for line in lines:
         if ":" in line:
-            name, line = (x.strip() for x in line.split(":", 1))
+            name, line = (x.strip() for x in line.split(":", 1))  # noqa: PLW2901
         if not line:
             continue
 
         if name is not None:
             if "=" in line:
                 key, value = (x.strip() for x in line.split("=", 1))
             else:
@@ -545,23 +545,27 @@
 
             if key == "logfile":
                 success = False
                 value = value.strip('"')
                 for p in path:
                     try:
                         # TODO: move on to use pathlib.
-                        logger.info(f"trying to read {os.path.join(p, value)}")
-                        compounds[name].update(read_logfile(os.path.join(p, value)))
+                        logger.info(
+                            f"trying to read {os.path.join(p, value)}",  # noqa: E501, G004, PTH118
+                        )
+                        compounds[name].update(
+                            read_logfile(os.path.join(p, value)),  # noqa: PTH118
+                        )
                     except FileNotFoundError:
                         continue
                     success = True
                     break
                 if not success:
-                    raise FileNotFoundError(
-                        f"could not find logfile '{value}' in path: {path}"  # noqa: E501, EM102
+                    raise FileNotFoundError(  # noqa: TRY003
+                        f"could not find logfile '{value}' in path: {path}",  # noqa: E501, EM102
                     )
             else:
                 # one-line JSON-encoded object
                 compounds[name][key] = json.loads(value)
     if select is not None:
         # TODO(schneiderfelipe): this workaround still allow unused compounds
         # to be parsed! This should change in the future.
@@ -641,29 +645,31 @@
                     (-0.721316, 1.137017, -4.3e-05)),
      'vibfreqs': (80.2535, 471.106, ..., 3129.0397, 3152.3619),
      'vibdisps': (((0.0, 0.0, 0.02),
                    ...,
                    (0.0, 0.0, 0.0)))}
     """
     if not (parser := ccopen(path)):
-        raise FileNotFoundError(f"could not find logfile '{path}'")  # noqa: EM102
+        raise FileNotFoundError(  # noqa: TRY003
+            f"could not find logfile '{path}'",  # noqa: EM102
+        )
     origin = parser.__class__.__name__.lower()
-    logger.info(f"reading a {origin} logfile: {path}")
+    logger.info(f"reading a {origin} logfile: {path}")  # noqa: G004
     try:
         ccdata = parser.parse()
         data = {
             "logfile": path,
             # This energy may lack dispersion, solvation, correlation, etc.
             "energy": ccdata.scfenergies[-1] * constants.eV * constants.N_A,
             "mult": ccdata.mult,
-            "atomnos": rx._misc.totuple(ccdata.atomnos),
-            "atommasses": rx._misc.totuple(ccdata.atommasses),
-            "atomcoords": rx._misc.totuple(ccdata.atomcoords[-1]),
-            "vibfreqs": rx._misc.totuple(ccdata.vibfreqs),
-            "vibdisps": rx._misc.totuple(ccdata.vibdisps),
+            "atomnos": rx._misc.totuple(ccdata.atomnos),  # noqa: SLF001
+            "atommasses": rx._misc.totuple(ccdata.atommasses),  # noqa: SLF001
+            "atomcoords": rx._misc.totuple(ccdata.atomcoords[-1]),  # noqa: SLF001
+            "vibfreqs": rx._misc.totuple(ccdata.vibfreqs),  # noqa: SLF001
+            "vibdisps": rx._misc.totuple(ccdata.vibdisps),  # noqa: SLF001
         }
 
         # This solves a current bug in cclib (see
         # https://github.com/cclib/cclib/issues/1080)
         if origin == "gaussian":
             data["atommasses"] = data["atommasses"][: len(data["atomnos"])]
 
@@ -681,16 +687,16 @@
             try:
                 # TODO(schneiderfelipe): only run the code below if we know it is
                 # an ORCA logfile. The code in this final section should be very
                 # specific in supplying *only* things cclib is not (yet) able to
                 # parse. Should we add a check for this as well?
                 data = _read_orca_logfile(path, minimal=False)
             except FileNotFoundError:
-                raise FileNotFoundError(  # noqa: B904
-                    f"could not parse logfile: '{path}'"  # noqa: EM102
+                raise FileNotFoundError(  # noqa: B904, TRY003, TRY200
+                    f"could not parse logfile: '{path}'",  # noqa: EM102
                 )  # noqa: RUF100
         else:
             raise
     return dotdict(data)
 
 
 def _read_orca_hess(path):
@@ -725,15 +731,15 @@
            [-0.01865457, -0.04015917, -0.01394534, -0.00232141,  0.02006353,
              0.0265781 ,  0.02097118,  0.0200932 , -0.01263546],
            [-0.01364819, -0.24287842, -0.25144318, -0.00644635,  0.00512802,
              0.01665733,  0.02009284,  0.237703  ,  0.23474131],
            [ 0.0160095 , -0.20678153, -0.26060801, -0.00337537, -0.02800411,
             -0.02595917, -0.01263597,  0.23474251,  0.28651783]])
     """
-    with open(path) as file:
+    with open(path) as file:  # noqa: PTH123
         while file:
             try:
                 line = next(file)
             except StopIteration:
                 break
 
             if line[:8] == "$hessian":
@@ -748,15 +754,15 @@
                         for j, entry in zip(columns, entries):
                             hessian[i, j] = float(entry)
                     line = next(file).strip()
         return hessian
 
 
 # heavily inspired by pieces of cclib
-def _read_orca_logfile(path, minimal=True):  # noqa: FBT002
+def _read_orca_logfile(path, minimal=True):  # noqa: C901, FBT002, PLR0915
     """Read an ORCA logfile.
 
     This function is a temporary reader, to be used until cclib supports all
     features we need. In particular, this function parses ORCA/xtb logfiles.
 
     Parameters
     ----------
@@ -796,15 +802,15 @@
      'atommasses': (35.453,),
      'vibfreqs': ()}
     """
     atomcoords = None
     atommasses = None
     vibfreqs = None
     hessian = None
-    with open(path) as file:
+    with open(path) as file:  # noqa: PTH123
         while file:
             try:
                 line = next(file)
             except StopIteration:
                 break
 
             if line[:25] == "FINAL SINGLE POINT ENERGY":
@@ -821,15 +827,15 @@
                     line = next(file)
 
                     atomnos = []
                     atomcoords = []
                     while len(line) > 1:
                         atom, x, y, z = line.split()
                         if atom[-1] != ">":
-                            atomnos.append(rx._misc.atomic_number[atom])
+                            atomnos.append(rx._misc.atomic_number[atom])  # noqa: SLF001
                             atomcoords.append([float(x), float(y), float(z)])
                         line = next(file)
 
                     natom = len(atomnos)
                 elif line[0:28] == "CARTESIAN COORDINATES (A.U.)":
                     next(file)
                     next(file)
@@ -870,52 +876,52 @@
                         # we have a single atom
                         vibfreqs = np.array([])
     data = {"energy": float(energy) * constants.hartree * constants.N_A}
 
     if hessian is None:
         try:
             hessian = _read_orca_hess(path.replace(".out", ".hess"))
-            data.update({"hessian": rx._misc.totuple(hessian)})
+            data.update({"hessian": rx._misc.totuple(hessian)})  # noqa: SLF001
         except FileNotFoundError:
             pass
 
     if minimal:
         return data
 
     # all non-minimal data is given below
     data.update({"logfile": path, "mult": int(mult)})
 
     if atomcoords is None:
-        with open(path.replace(".out", ".xyz")) as file:
+        with open(path.replace(".out", ".xyz")) as file:  # noqa: PTH123
             n = int(next(file))
             next(file)
 
             atomnos = []
             atomcoords = []
             for _ in range(n):
                 line = next(file)
                 atom, x, y, z = line.split()
-                atomnos.append(rx._misc.atomic_number[atom])
+                atomnos.append(rx._misc.atomic_number[atom])  # noqa: SLF001
                 atomcoords.append([float(x), float(y), float(z)])
     data.update(
         {
-            "atomnos": rx._misc.totuple(atomnos),
-            "atomcoords": rx._misc.totuple(atomcoords),
-        }
+            "atomnos": rx._misc.totuple(atomnos),  # noqa: SLF001
+            "atomcoords": rx._misc.totuple(atomcoords),  # noqa: SLF001
+        },
     )
 
     if atommasses is None:
         logger.warning("using atomic masses from periodic table")
         atommasses = []
         for n in atomnos:
-            atommasses.append(rx._misc.atomic_mass[n])
-    data.update({"atommasses": rx._misc.totuple(atommasses)})
+            atommasses.append(rx._misc.atomic_mass[n])  # noqa: SLF001
+    data.update({"atommasses": rx._misc.totuple(atommasses)})  # noqa: SLF001
 
     if vibfreqs is not None:
-        data.update({"vibfreqs": rx._misc.totuple(vibfreqs)})
+        data.update({"vibfreqs": rx._misc.totuple(vibfreqs)})  # noqa: SLF001
 
     return data
 
 
 # https://stackoverflow.com/a/23689767/4039050
 class dotdict(dict):  # noqa: N801
     """Access dictionary attributes through dot.notation.
@@ -947,44 +953,46 @@
     """
 
     def __init__(self, *args, **kwargs) -> None:  # noqa: ANN101, ANN002, ANN003
         super().__init__(*args, **kwargs)
 
         for key, val in self.items():
             if isinstance(val, (list, np.ndarray)):
-                super().__setitem__(key, rx._misc.totuple(val))
+                super().__setitem__(key, rx._misc.totuple(val))  # noqa: SLF001
             elif isinstance(val, dict):
                 super().__setitem__(key, dotdict(val))
 
     __getattr__ = dict.get
 
-    def __setitem__(self, key, value):  # noqa: ANN101, ARG002, ANN204
+    def __setitem__(self, key, value):  # noqa: ANN101, ANN204
         """
         Set an item.
 
         This is not allowed and will raise an exception.
 
         Raises
         ------
         NotImplementedError
             If one attempts to change a value.
         """
-        raise NotImplementedError("dotdict objects are immutable")  # noqa: EM101
+        raise NotImplementedError(  # noqa: TRY003
+            "dotdict objects are immutable",  # noqa: EM101
+        )
 
     # https://stackoverflow.com/a/1151686/4039050
     # https://stackoverflow.com/a/1151705/4039050
     def __hash__(self):  # noqa: ANN101, ANN204, D105
         return hash(self._key())
 
     # https://stackoverflow.com/a/16162138/4039050
     def _key(self):  # noqa: ANN101
         return (frozenset(self), frozenset(self.items()))
 
     def __eq__(self, other):  # noqa: ANN101, ANN204, D105
-        return self._key() == other._key()
+        return self._key() == other._key()  # noqa: SLF001
 
 
 # https://stackoverflow.com/a/61144084/4039050
 class _LazyDict(MutableMapping):
     """Lazily evaluated dictionary."""
 
     _function = None
@@ -996,15 +1004,15 @@
         """Evaluate value."""
         value = self._dict[key]
         if not isinstance(value, dict):
             data = self._function(value)
 
             value = data
             self._dict[key] = data
-        return value  # noqa: RET504
+        return value
 
     def __setitem__(self, key, value):  # noqa: ANN101, ANN204
         """Store value lazily."""
         self._dict[key] = value
 
     def __delitem__(self, key):  # noqa: ANN101, ANN204
         """Delete value."""
```

### Comparing `overreact-1.1.0/overreact/rates.py` & `overreact-1.2.0/overreact/rates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python3  # noqa: EXE001
 
 """Module dedicated to the calculation of reaction rate constants."""
 
 
 from __future__ import annotations
 
 __all__ = ["eyring"]
@@ -39,19 +39,19 @@
         Dynamic viscosity in SI units (Pa*s).
 
     Examples
     --------
     >>> liquid_viscosity("water", temperature=299.26)
     8.90e-4
     """
-    return rx._misc._get_chemical(id, temperature, pressure).mul
+    return rx._misc._get_chemical(id, temperature, pressure).mul  # noqa: SLF001
 
 
 # TODO(schneiderfelipe): log the calculated diffusional reaction rate limit.
-def smoluchowski(
+def smoluchowski(  # noqa: PLR0913
     radii,
     viscosity=None,
     reactive_radius=None,
     temperature=298.15,
     pressure=constants.atm,
     mutual_diff_coef=None,
 ):
@@ -137,15 +137,15 @@
     --------
     >>> collins_kimball(2.3e7, 3.6e9)
     2.3e7
     """
     return k_tst * k_diff / (k_tst + k_diff)
 
 
-def convert_rate_constant(  # noqa: C901
+def convert_rate_constant(  # noqa: C901, PLR0912, PLR0913
     val,
     new_scale,
     old_scale="l mol-1 s-1",
     molecularity=1,
     temperature=298.15,
     pressure=constants.atm,
 ):
@@ -249,15 +249,15 @@
             * pressure
             * constants.kilo
             / constants.torr
         )
     elif old_scale == "atm-1 s-1":
         factor = rx.thermo.molar_volume(temperature, pressure) * constants.kilo
     else:
-        raise ValueError(f"old unit not recognized: {old_scale}")  # noqa: EM102
+        raise ValueError(f"old unit not recognized: {old_scale}")  # noqa: EM102, TRY003
 
     # now we convert l mol-1 s-1 to what we need
     if new_scale == "cm3 mol-1 s-1":
         factor *= constants.kilo
     elif new_scale == "l mol-1 s-1":
         factor *= 1.0
     elif new_scale == "m3 mol-1 s-1":
@@ -267,18 +267,20 @@
     elif new_scale == "mmHg-1 s-1":
         factor *= constants.torr / (
             rx.thermo.molar_volume(temperature, pressure) * pressure * constants.kilo
         )
     elif new_scale == "atm-1 s-1":
         factor *= 1.0 / (rx.thermo.molar_volume(temperature, pressure) * constants.kilo)
     else:
-        raise ValueError(f"new unit not recognized: {new_scale}")  # noqa: EM102
+        raise ValueError(f"new unit not recognized: {new_scale}")  # noqa: EM102, TRY003
 
     factor **= molecularity - 1
-    logger.info(f"conversion factor ({old_scale} to {new_scale}) = {factor}")
+    logger.info(
+        f"conversion factor ({old_scale} to {new_scale}) = {factor}",  # noqa: G004
+    )
     return val * factor
 
 
 def eyring(
     delta_freeenergy: Union[float, np.ndarray],  # noqa: UP007
     molecularity: Optional[int] = None,  # noqa: UP007
     temperature: Union[float, np.ndarray] = 298.15,  # noqa: UP007
@@ -361,13 +363,17 @@
 
     delta_moles = None
     if molecularity is not None:
         delta_moles = 1 - np.asarray(molecularity)
 
     return (
         rx.thermo.equilibrium_constant(
-            delta_freeenergy, delta_moles, temperature, pressure, volume
+            delta_freeenergy,
+            delta_moles,
+            temperature,
+            pressure,
+            volume,
         )
         * constants.k
         * temperature
         / constants.h
     )
```

### Comparing `overreact-1.1.0/overreact/simulate.py` & `overreact-1.2.0/overreact/simulate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python3  # noqa: EXE001
 
 """Module dedicated to the time simulation of reaction models.
 
 Here are functions that calculate reaction rates as well, which is needed for
 the time simulations.
 """
 
@@ -46,25 +46,27 @@
     from jax import jacfwd, jit
     from jax.config import config
 
     config.update("jax_enable_x64", True)  # noqa: FBT003
 else:
     logger.warning(
         "Install JAX to have just-in-time compilation: "
-        'pip install jax (or pip install "overreact[fast]")'
+        'pip install jax (or pip install "overreact[fast]")',
     )
     jnp = np
 
 
 # TODO(schneiderfelipe): allow y0 to be a dict-like object.
-def get_y(
+def get_y(  # noqa: PLR0913
     dydt,
     y0,
     t_span=None,
-    method="LSODA",
+    method="RK23",
+    max_step=np.inf,
+    first_step=np.finfo(np.float64).eps,  # noqa: B008
     rtol=1e-3,
     atol=1e-6,
     max_time=1 * 60 * 60,
 ):
     """Simulate a reaction scheme from its rate function.
 
     This function provides two functions that calculate the concentrations and
@@ -81,17 +83,24 @@
     t_span : array-like, optional
         Interval of integration (t0, tf). The solver starts with t=t0 and
         integrates until it reaches t=tf. If not given, a conservative value
         is chosen based on the system at hand (the method of choice works for
         any zeroth-, first- or second-order reactions).
     method : str, optional
         Integration method to use. See `scipy.integrate.solve_ivp` for details.
-        Kinetics problems are very often stiff and, as such, "RK45" is
-        normally unsuited. "Radau", "BDF" or "LSODA" are good choices.
-    rtol, atol : array-like
+        Kinetics problems are very often stiff and, as such, "RK23" and "RK45" may be
+        unsuited. "LSODA", "BDF", and "Radau" are worth a try if things go bad.
+    max_step : float, optional
+        Maximum step to be performed by the integrator.
+        Defaults to half the total time span.
+    first_step : float, optional
+        First step size.
+        Defaults to half the maximum step, or `np.finfo(np.float64).eps`,
+        whichever is smallest.
+    rtol, atol : array-like, optional
         See `scipy.integrate.solve_ivp` for details.
     max_time : float, optional
         If `t_span` is not given, an interval will be estimated, but it can't
         be larger than this parameter.
 
     Returns
     -------
@@ -109,29 +118,29 @@
 
     >>> scheme = rx.parse_reactions("A <=> B")
     >>> y, r = get_y(get_dydt(scheme, np.array([1, 1])), y0=[1, 0])
 
     The `y` object stores information about the simulation time, which can be
     used to produce a suitable vector of timepoints for, e.g., plotting:
 
-    >>> y.t_min, y.t_max  # doctest: +SKIP
+    >>> y.t_min, y.t_max
     (0.0, 3.0)
     >>> t = np.linspace(y.t_min, y.t_max)
-    >>> t  # doctest: +SKIP
+    >>> t
     array([0. , 0.06122449, ..., 2.93877551, 3. ])
 
     Both `y` and `r` can be used to check concentrations and rates in any
     point in time. In particular, both are vectorized:
 
-    >>> y(t)  # doctest: +SKIP
-    array([[1. , 0.94237559, ..., 0.5012394, 0.5 ],
-           [0. , 0.05762441, ..., 0.4987606, 0.5 ]])
-    >>> r(t)  # doctest: +SKIP
-    array([[-1.00000000e+00, ..., -1.39544265e-10],
-           [ 1.00000000e+00, ...,  1.39544265e-10]])
+    >>> y(t)
+    array([[1. , ...],
+           [0. , ...]])
+    >>> r(t)
+    array([[-1. , ...],
+           [ 1. , ...]])
     """
     # TODO(schneiderfelipe): raise a meaningful error when y0 has the wrong shape.
     y0 = np.asarray(y0)
 
     if t_span is None:
         # We defined alpha such that 1.0 - alpha is an (under)estimate of the extend
         # to which the reaction is simulated. And then we apply the Pareto principle.
@@ -141,65 +150,43 @@
         halflife_estimate = 1.0
         if hasattr(dydt, "k"):
             halflife_estimate = np.max(
                 [
                     np.max(y0) / 2.0,  # zeroth-order halflife
                     np.log(2.0),  # first-order halflife
                     1.0 / np.min(y0[np.nonzero(y0)]),  # second-order halflife
-                ]
+                ],
             ) / np.min(dydt.k)
-            logger.info(f"largest halflife guess = {halflife_estimate} s")
+            logger.info(f"largest halflife guess = {halflife_estimate} s")  # noqa: G004
 
         t_span = [0.0, min(n_halflives * halflife_estimate, max_time)]
-        logger.info(f"simulation time span   = {t_span} s")
+        logger.info(f"simulation time span   = {t_span} s")  # noqa: G004
 
-    jac = None
-    if hasattr(dydt, "jac"):
-        jac = dydt.jac
+    max_step = np.min([max_step, (t_span[1] - t_span[0]) / 2.0])
+    logger.warning(f"max step = {max_step} s")  # noqa: G004
 
-    # This should be small enough.
-    # It seems to be required by LSODA, but has no visible effect on Radau.
-    # I don't care about BDF.
-    #
-    # Estimates are based on
-    # - the estimated time it takes for hydrogen atoms bind to a graphene sheet,
-    # - the diffusion constant of n-pentane,
-    # - the reaction rate of H2CO3 dehydration by carbonic anhydrase,
-    # - the hundredth part of the timespan,
-    # - some numberical limits,
-    first_step = np.min(
-        [
-            1e-14,  # Too small?
-            1 / 27e9,  # Too small?
-            1 / 1.5e10,
-            (t_span[1] - t_span[0]) / 100.0,
-            np.finfo(np.float16).eps,
-            np.finfo(np.float32).eps,
-            np.finfo(np.float64).eps,  # Too small?
-            np.nextafter(np.float16(0), np.float16(1)),
-        ]
-    )
-    logger.warning(f"first step = {first_step} s")
+    first_step = np.min([first_step, max_step / 2.0])
+    logger.warning(f"first step = {first_step} s")  # noqa: G004
 
-    # Too large a max step breaks LSODA. A too small one breaks it too.
-    max_step = np.min([1.0, (t_span[1] - t_span[0]) / 100.0])
-    logger.warning(f"max step = {max_step} s")
+    jac = None
+    if hasattr(dydt, "jac"):
+        jac = dydt.jac  # noqa: F841
 
-    logger.warning(f"@t = \x1b[94m{0:10.3f} \x1b[ms\x1b[K")
+    logger.warning(f"@t = \x1b[94m{0:10.3f} \x1b[ms\x1b[K")  # noqa: G004
     res = solve_ivp(
         dydt,
         t_span,
         y0,
         method=method,
         dense_output=True,
-        first_step=first_step,
         max_step=max_step,
+        first_step=first_step,
         rtol=rtol,
         atol=atol,
-        jac=jac,
+        # jac=jac,  # noqa: ERA001
     )
     logger.warning(res)
     y = res.sol
 
     def r(t):
         # TODO(schneiderfelipe): this is probably not the best way to
         # vectorize a function!
@@ -246,36 +233,36 @@
     Examples
     --------
     >>> import numpy as np
     >>> import overreact as rx
 
     >>> scheme = rx.parse_reactions("A <=> B")
     >>> dydt = get_dydt(scheme, np.array([1, 1]))
-    >>> dydt(0.0, np.array([1., 1.]))  # doctest: +SKIP
-    array([0., 0.])
+    >>> dydt(0.0, np.array([1., 1.]))
+    Array([0., 0.], ...)
 
     If available, JAX is used for JIT compilation. This will make `dydt`
     complain if given lists instead of numpy arrays. So stick to the safer,
     faster side as above.
 
     The actually used reaction rate constants can be inspected with the `k`
     attribute of `dydt`:
 
-    >>> dydt.k  # doctest: +SKIP
-    array([1., 1.])
+    >>> dydt.k
+    Array([1., 1.], ...)
 
     If JAX is available, the Jacobian function will be available as
     `dydt.jac`:
 
-    >>> dydt.jac(0.0, np.array([1., 1.]))  # doctest: +SKIP
-    DeviceArray([[-1.,  1.],
-                 [ 1., -1.]], dtype=float64)
+    >>> dydt.jac(0.0, np.array([1., 1.]))
+    Array([[-1.,  1.],
+           [ 1., -1.]], ...)
 
     """
-    scheme = rx.core._check_scheme(scheme)
+    scheme = rx.core._check_scheme(scheme)  # noqa: SLF001
     A = jnp.asarray(scheme.A)  # noqa: N806
     M = jnp.where(A > 0, 0, -A).T  # noqa: N806
     k_adj = _adjust_k(scheme, k, ef=ef)
 
     def _dydt(t, y):  # noqa: ARG001
         r = k_adj * jnp.prod(jnp.power(y, M), axis=1)
         return jnp.dot(A, r)
@@ -284,15 +271,15 @@
         # Using JAX for JIT compilation is much faster.
         _dydt = jit(_dydt)
 
         # NOTE(schneiderfelipe): the following function is defined
         # such that _jac(t, y)[i, j] == d f_i / d y_j,
         # with shape of (n_compounds, n_compounds).
         def _jac(t, y):
-            logger.warning(f"\x1b[A@t = \x1b[94m{t:10.3f} \x1b[ms\x1b[K")
+            logger.warning(f"\x1b[A@t = \x1b[94m{t:10.3f} \x1b[ms\x1b[K")  # noqa: G004
             return jacfwd(lambda _y: _dydt(t, _y))(y)
 
         _dydt.jac = _jac
 
     _dydt.k = k_adj
     return _dydt
 
@@ -320,55 +307,57 @@
         Adjusted constants.
 
     Examples
     --------
     >>> import overreact as rx
 
     >>> scheme = rx.parse_reactions("A <=> B")
-    >>> _adjust_k(scheme, [1, 1])  # doctest: +SKIP
-    array([1., 1.])
+    >>> _adjust_k(scheme, [1, 1])
+    Array([1., 1.], ...)
 
     >>> model = rx.parse_model("data/ethane/B97-3c/model.k")
     >>> _adjust_k(model.scheme,
-    ...           rx.get_k(model.scheme, model.compounds))  # doctest: +SKIP
-    array([8.16880917e+10])
+    ...           rx.get_k(model.scheme, model.compounds))
+    Array([8.16880917e+10], ...)
 
     >>> model = rx.parse_model("data/acetate/Orca4/model.k")
     >>> _adjust_k(model.scheme,
-    ...           rx.get_k(model.scheme, model.compounds))  # doctest: +SKIP
-    array([1.00000000e+00, 5.74491548e+04, 1.61152010e+07,
-           1.00000000e+00, 1.55695112e+56, 1.00000000e+00])
+    ...           rx.get_k(model.scheme, model.compounds))
+    Array([1.00000000e+00, 5.74491548e+04, 1.61152010e+07,
+           1.00000000e+00, 1.55695112e+56, 1.00000000e+00], ...)
 
     >>> model = rx.parse_model(
     ...     "data/perez-soto2020/RI/BLYP-D4/def2-TZVP/model.k"
     ... )
     >>> _adjust_k(model.scheme,
-    ...           rx.get_k(model.scheme, model.compounds))  # doctest: +SKIP
-    array([1.02320357e+12, ..., 1.02320357e+12])
+    ...           rx.get_k(model.scheme, model.compounds))
+    Array([...], ...)
 
     """
-    scheme = rx.core._check_scheme(scheme)
+    scheme = rx.core._check_scheme(scheme)  # noqa: SLF001
     is_half_equilibrium = np.asarray(scheme.is_half_equilibrium)
-    k = np.asarray(k, dtype=float).copy()
+    k = np.asarray(k, dtype=np.float64).copy()
 
     if np.any(is_half_equilibrium):
         # at least one equilibrium
         if np.any(~is_half_equilibrium):
             # at least one true reaction
 
             k_slowest_equil = k[is_half_equilibrium].min()
             k_fastest_react = k[~is_half_equilibrium].max()
             adjustment = ef * (k_fastest_react / k_slowest_equil)
 
             k[is_half_equilibrium] *= adjustment
-            logger.warning(f"equilibria adjustment = {adjustment}")
+            logger.warning(f"equilibria adjustment = {adjustment}")  # noqa: G004
 
             k_slowest_equil = k[is_half_equilibrium].min()
             k_fastest_react = k[~is_half_equilibrium].max()
-            logger.warning(f"slow eq. / fast r. = {k_slowest_equil / k_fastest_react}")
+            logger.warning(
+                f"slow eq. / fast r. = {k_slowest_equil / k_fastest_react}",  # noqa: E501, G004
+            )
         else:
             # only equilibria
 
             # set the smallest one to be equal to one
             k = k / k.min()
 
     return jnp.asarray(k)
@@ -524,20 +513,22 @@
     >>> new_scheme, new_k = rx.get_fixed_scheme(scheme, k, {})
     >>> new_scheme == scheme
     True
     >>> np.allclose(new_k, k)
     True
 
     """
-    new_k = np.asarray(k, dtype=float).copy()
+    new_k = np.asarray(k, dtype=np.float64).copy()
     new_reactions = []
     for i, (reaction, is_half_equilibrium) in enumerate(
-        zip(scheme.reactions, scheme.is_half_equilibrium)
+        zip(scheme.reactions, scheme.is_half_equilibrium),
     ):
-        for reactants, products, _ in rx.core._parse_reactions(reaction):
+        for reactants, products, _ in rx.core._parse_reactions(  # noqa: SLF001
+            reaction,
+        ):
             new_reactants = tuple(
                 (coeff, compound)
                 for (coeff, compound) in reactants
                 if compound not in fixed_y0
             )
             new_products = tuple(
                 (coeff, compound)
@@ -548,22 +539,26 @@
             for fixed_compound in fixed_y0:
                 for coeff, compound in reactants:
                     if fixed_compound == compound:
                         new_k[i] *= fixed_y0[fixed_compound] ** coeff
 
             new_reactions.append((new_reactants, new_products, is_half_equilibrium))
 
-    new_reactions = tuple(r for r in rx.core._unparse_reactions(new_reactions))
+    new_reactions = tuple(
+        r for r in rx.core._unparse_reactions(new_reactions)  # noqa: SLF001
+    )  # noqa: RUF100, SLF001
     new_is_half_equilibrium = scheme.is_half_equilibrium
 
     new_A = []  # noqa: N806
     new_B = []  # noqa: N806
     new_compounds = []
     for compound, row_A, row_B in zip(  # noqa: N806
-        scheme.compounds, scheme.A, scheme.B
+        scheme.compounds,
+        scheme.A,
+        scheme.B,
     ):  # noqa: RUF100
         if compound not in fixed_y0:
             new_compounds.append(compound)
             new_A.append(row_A)
             new_B.append(row_B)
 
     new_compounds = tuple(new_compounds)
@@ -579,24 +574,24 @@
             B=new_B,
         ),
         new_k,
     )
 
 
 # TODO(schneiderfelipe): this is probably not ready yet
-def get_bias(
+def get_bias(  # noqa: PLR0913
     scheme,
     compounds,
     data,
     y0,
     tunneling="eckart",
     qrrho=True,  # noqa: FBT002
     temperature=298.15,
     pressure=constants.atm,
-    method="LSODA",
+    method="RK23",
     rtol=1e-3,
     atol=1e-6,
 ):
     r"""Estimate a energy bias for a given set of reference data points.
 
     Parameters
     ----------
@@ -650,16 +645,16 @@
     ...       2.7426565371219e-5]
     >>> data = {"t": [1.276472128376942246e-6,
     ...               1.446535794555581743e-4,
     ...               1.717069678525567564e-2],
     ...         "CH3·": [9.694916853338366211e-9,
     ...                  1.066033349343709026e-6,
     ...                  2.632179124780495175e-5]}
-    >>> get_bias(model.scheme, model.compounds, data, y0) / constants.kcal  # doctest: +SKIP
-    -1.36
+    >>> get_bias(model.scheme, model.compounds, data, y0) / constants.kcal
+    -1.4
     """  # noqa: E501
     max_time = np.max(data["t"])
 
     def f(bias):
         k = rx.get_k(
             scheme,
             compounds,
@@ -669,21 +664,26 @@
             temperature=temperature,
             pressure=pressure,
         )
 
         # TODO(schneiderfelipe): support schemes with fixed concentrations
         dydt = rx.get_dydt(scheme, k)
         y, _ = rx.get_y(
-            dydt, y0=y0, method=method, rtol=rtol, atol=atol, max_time=max_time
+            dydt,
+            y0=y0,
+            method=method,
+            rtol=rtol,
+            atol=atol,
+            max_time=max_time,
         )
 
         yhat = y(data["t"])
         return np.sum(
             [
                 (yhat[i] - data[name]) ** 2
                 for (i, name) in enumerate(compounds)
                 if name in data
-            ]
+            ],
         )
 
     res = minimize_scalar(f)
     return res.x
```

### Comparing `overreact-1.1.0/overreact/thermo/__init__.py` & `overreact-1.2.0/overreact/thermo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python3  # noqa: EXE001
 
 """Module dedicated to the calculation of thermodynamic properties."""
 
 
 from __future__ import annotations
 
 __all__ = ["equilibrium_constant", "change_reference_state"]
@@ -27,15 +27,15 @@
     calc_vib_entropy,
     molar_volume,
 )
 
 logger = logging.getLogger(__name__)
 
 
-def calc_trans_entropy(
+def calc_trans_entropy(  # noqa: PLR0913
     atommasses,
     atomnos=None,
     atomcoords=None,
     environment="gas",
     method="standard",
     temperature=298.15,
     pressure=constants.atm,
@@ -100,52 +100,56 @@
     >>> calc_trans_entropy(35.45, [17], [[0, 0, 0]], environment="water",
     ...                    method="izato")
     51.
 
     >>> calc_trans_entropy(35.45, [17], [[0, 0, 0]], environment="benzene",
     ...                    method="garza")
     121.7
-    """  # noqa: E501
+    """
     # TODO(schneiderfelipe): This is probably an ugly hack for zero temperature and
     # certainly wrong (https://physics.stackexchange.com/a/400431/77366).
     # See https://physics.stackexchange.com/a/468649/77366 and
     # https://physics.stackexchange.com/a/335828/77366 for further details on what we
     # should do (disclaimer: no Sackur-Tetrode at 0 K!).
     if np.isclose(temperature, 0.0):
         logger.warning("assuming translational entropy zero at zero temperature")
         return 0.0
 
     if environment in {"gas", None} or method == "standard":
         volume = molar_volume(temperature=temperature, pressure=pressure)
-    elif environment == "solid":  # noqa: RET506
-        raise ValueError(
-            f"environment not yet implemented: {environment}"  # noqa: EM102
+    elif environment == "solid":
+        raise ValueError(  # noqa: TRY003
+            f"environment not yet implemented: {environment}",  # noqa: EM102
         )  # noqa: RUF100
     else:
         assert atomnos is not None, "atomnos must be provided"
         assert atomcoords is not None, "atomcoords must be provided"
-        volume = rx.thermo._solv.molar_free_volume(
+        volume = rx.thermo._solv.molar_free_volume(  # noqa: SLF001
             atomnos=atomnos,
             atomcoords=atomcoords,
             environment=environment,
             method=method,
             temperature=temperature,
             pressure=pressure,
         )
 
-    translational_entropy = rx.thermo._gas._sackur_tetrode(
-        atommasses, volume, temperature=temperature
+    translational_entropy = rx.thermo._gas._sackur_tetrode(  # noqa: SLF001
+        atommasses,
+        volume,
+        temperature=temperature,
+    )
+    logger.info(
+        f"translational entropy = {translational_entropy} J/mol·K",  # noqa: G004
     )
-    logger.info(f"translational entropy = {translational_entropy} J/mol·K")
     return translational_entropy
 
 
 # TODO(schneiderfelipe): "energy" has potentially two meanings here. Correct
 # naming for the whole package?
-def calc_internal_energy(
+def calc_internal_energy(  # noqa: PLR0913
     energy=0.0,
     degeneracy=1,
     moments=None,
     vibfreqs=None,
     qrrho=True,  # noqa: FBT002
     temperature=298.15,
 ):
@@ -199,21 +203,21 @@
     """  # noqa: E501
     internal_energy = (
         calc_trans_energy(temperature=temperature)
         + calc_elec_energy(energy, degeneracy, temperature=temperature)
         + calc_rot_energy(moments, temperature=temperature)
         + calc_vib_energy(vibfreqs, qrrho=qrrho, temperature=temperature)
     )
-    logger.info(f"internal energy = {internal_energy} J/mol")
+    logger.info(f"internal energy = {internal_energy} J/mol")  # noqa: G004
     return internal_energy
 
 
 # TODO(schneiderfelipe): "energy" has potentially two meanings here. Correct
 # naming for the whole package?
-def calc_enthalpy(
+def calc_enthalpy(  # noqa: PLR0913
     energy=0.0,
     degeneracy=1,
     moments=None,
     vibfreqs=None,
     qrrho=True,  # noqa: FBT002
     temperature=298.15,
 ):
@@ -275,21 +279,21 @@
             moments=moments,
             vibfreqs=vibfreqs,
             qrrho=qrrho,
             temperature=temperature,
         )
         + constants.R * temperature
     )
-    logger.info(f"enthalpy = {enthalpy} J/mol")
+    logger.info(f"enthalpy = {enthalpy} J/mol")  # noqa: G004
     return enthalpy
 
 
 # TODO(schneiderfelipe): "energy" has potentially two meanings here. Correct
 # naming for the whole package?
-def calc_entropy(
+def calc_entropy(  # noqa: PLR0913
     atommasses,
     atomnos=None,
     atomcoords=None,
     energy=0.0,
     degeneracy=1,
     moments=None,
     symmetry_number=1,
@@ -399,15 +403,17 @@
             atomcoords=atomcoords,
             environment=environment,
             method=method,
             temperature=temperature,
             pressure=pressure,
         )
         + calc_elec_entropy(
-            energy=energy, degeneracy=degeneracy, temperature=temperature
+            energy=energy,
+            degeneracy=degeneracy,
+            temperature=temperature,
         )
         + calc_rot_entropy(
             atommasses=atommasses,
             atomnos=atomnos,
             atomcoords=atomcoords,
             moments=moments,
             symmetry_number=symmetry_number,
@@ -417,43 +423,46 @@
             pressure=pressure,
         )
         + calc_vib_entropy(vibfreqs=vibfreqs, qrrho=qrrho, temperature=temperature)
     )
 
     if environment in {"gas", None}:
         pass
-    elif environment == "solid":  # noqa: RET506
-        raise ValueError(
-            f"environment not yet implemented: {environment}"  # noqa: EM102
+    elif environment == "solid":
+        raise ValueError(  # noqa: TRY003
+            f"environment not yet implemented: {environment}",  # noqa: EM102
         )  # noqa: RUF100
     else:
         concentration_correction = -change_reference_state(
-            temperature=temperature, pressure=pressure
+            temperature=temperature,
+            pressure=pressure,
+        )
+        logger.debug(
+            f"concentration correction = {concentration_correction} J/mol·K",  # noqa: E501, G004
         )
-        logger.debug(f"concentration correction = {concentration_correction} J/mol·K")
         entropy = entropy + concentration_correction
         if method == "standard":
             pass
         else:
             assert atomnos is not None, "atomnos must be provided"
             assert atomcoords is not None, "atomcoords must be provided"
             # TODO(schneiderfelipe): this includes "izato", "garza" and
             # possibly future methods for extra entropy terms such as cavity.
-            entropy = entropy + rx.thermo._solv.calc_cav_entropy(
+            entropy = entropy + rx.thermo._solv.calc_cav_entropy(  # noqa: SLF001
                 atomnos=atomnos,
                 atomcoords=atomcoords,
                 environment=environment,
                 temperature=temperature,
                 pressure=pressure,
             )  # TODO(schneiderfelipe): check extra options for calc_cav_entropy.
-    logger.info(f"entropy = {entropy} J/mol·K")
+    logger.info(f"entropy = {entropy} J/mol·K")  # noqa: G004
     return entropy
 
 
-def calc_heat_capacity(
+def calc_heat_capacity(  # noqa: PLR0913
     energy=0.0,
     degeneracy=1,
     moments=None,
     vibfreqs=None,
     qrrho=True,  # noqa: FBT002
     temperature=298.15,
     dx=3e-5,
@@ -506,28 +515,28 @@
     >>> energy = np.array([0.000, 404.141, 102405.714, 102680.439,  # cm-1
     ...                    102840.378, 104731.048, 105056.283])
     >>> calc_heat_capacity(
     ...     energy=energy * 100 * constants.h * constants.c * constants.N_A,
     ...     degeneracy=degeneracy)  # F
     14.43
 
-    """  # noqa: D202, E501
+    """  # noqa: E501
 
     def func(temperature):
         return calc_internal_energy(
             energy=energy,
             degeneracy=degeneracy,
             moments=moments,
             vibfreqs=vibfreqs,
             qrrho=qrrho,
             temperature=temperature,
         )
 
     heat_capacity = derivative(func, x0=temperature, dx=dx, n=1, order=order)
-    logger.info(f"heat capacity = {heat_capacity} J/mol·K")
+    logger.info(f"heat capacity = {heat_capacity} J/mol·K")  # noqa: G004
     return heat_capacity
 
 
 def get_molecularity(transform):
     """Calculate molecularity of a chemical transformation.
 
     The returned value is the reaction order, i.e., number of molecules that come
@@ -730,32 +739,32 @@
     >>> np.log10(equilibrium_constant(dG1, delta_moles=-4))
     array([0.998])
     >>> np.log10(equilibrium_constant(dG2, delta_moles=-2))
     array([7.85])
 
     You can easily check that the above values match the values given
     [here](https://en.wikipedia.org/wiki/Stability_constants_of_complexes#The_chelate_effect).
-    """  # noqa: E501
+    """
     temperature = np.asarray(temperature)
 
     equilibrium_constant = np.exp(
-        -np.atleast_1d(delta_freeenergy) / (constants.R * temperature)
+        -np.atleast_1d(delta_freeenergy) / (constants.R * temperature),
     )
 
     if delta_moles is not None:
         if volume is None:
             volume = molar_volume(temperature, pressure) * constants.kilo
 
         equilibrium_constant *= volume**delta_moles
 
-    logger.info(f"equilibrium constant = {equilibrium_constant}")
+    logger.info(f"equilibrium constant = {equilibrium_constant}")  # noqa: G004
     return equilibrium_constant
 
 
-def change_reference_state(
+def change_reference_state(  # noqa: PLR0913
     new_reference: float = 1.0 / constants.liter,
     old_reference: Optional[float] = None,  # noqa: UP007
     sign: int = 1,
     temperature: Union[float, np.ndarray] = 298.15,  # noqa: UP007
     pressure: float = constants.atm,
     volume: Optional[float] = None,  # noqa: UP007
 ):
```

### Comparing `overreact-1.1.0/overreact/thermo/_gas.py` & `overreact-1.2.0/overreact/thermo/_gas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python3  # noqa: EXE001
 
 """Module dedicated to the calculation of thermodynamic properties in gas phase."""
 
 import logging
 
 import numpy as np
 
@@ -34,15 +34,15 @@
     >>> calc_trans_energy(373.15)
     4653.
 
     """
     temperature = np.asarray(temperature)
 
     translational_energy = 1.5 * constants.R * temperature
-    logger.info(f"translational energy = {translational_energy} J/mol")
+    logger.info(f"translational energy = {translational_energy} J/mol")  # noqa: G004
     return translational_energy
 
 
 def calc_elec_energy(energy=0.0, degeneracy=1, temperature=298.15):
     """Calculate electronic energy.
 
     This eventually adds a correction based on accessible excited states, but
@@ -105,15 +105,15 @@
         return min_energy
 
     energy = energy - min_energy
     q_elec_terms = degeneracy * np.exp(-energy / (constants.R * temperature))
     q_elec = np.sum(q_elec_terms)
 
     electronic_energy = min_energy + np.sum(energy * q_elec_terms) / q_elec
-    logger.info(f"electronic energy = {electronic_energy} J/mol")
+    logger.info(f"electronic energy = {electronic_energy} J/mol")  # noqa: G004
     return electronic_energy
 
 
 def calc_elec_entropy(energy=0.0, degeneracy=1, temperature=298.15):
     """Calculate electronic entropy.
 
     This eventually adds a correction based on accessible excited states, but
@@ -183,22 +183,25 @@
     min_energy = np.asarray(energy).min()
     energy = energy - min_energy
 
     q_elec_terms = degeneracy * np.exp(-energy / (constants.R * temperature))
     q_elec = np.sum(q_elec_terms)
 
     electronic_entropy = constants.R * np.log(q_elec) + np.sum(
-        energy * q_elec_terms
+        energy * q_elec_terms,
     ) / (temperature * q_elec)
-    logger.info(f"electronic entropy = {electronic_entropy} J/mol·K")
+    logger.info(f"electronic entropy = {electronic_entropy} J/mol·K")  # noqa: G004
     return electronic_entropy
 
 
 def calc_rot_energy(
-    moments=None, independent=False, weights=1.0, temperature=298.15  # noqa: FBT002
+    moments=None,
+    independent=False,  # noqa: FBT002
+    weights=1.0,
+    temperature=298.15,
 ):  # noqa: RUF100
     r"""Calculate the rotational energy of an ideal gas.
 
     This function uses the truncation of equation 6-48 of Statistical
     Thermodynamics, McQuarrie, which is valid for temperatures larger than five
     times the rotational temperatures and correct up to second order in the
     inverse temperature. Observe that this is more precise than equation 8-20
@@ -237,50 +240,47 @@
     3674.
 
     If no moments of inertia are given, a monoatomic gas is assumed:
 
     >>> calc_rot_energy()
     0.0
 
-    """  # noqa: E501
+    """
     temperature = np.asarray(temperature)
 
     if np.isclose(temperature, 0.0):
         logger.warning("assuming rotational energy zero at zero temperature")
         return 0.0
 
     rotational_temperatures = _rotational_temperature(moments)
     if not rotational_temperatures.size:
         logger.warning("assuming zero rotational energy for atomic system")
         return 0.0
 
     if not independent and np.any(rotational_temperatures >= 0.2 * temperature):
         logger.warning(
-            f"rotational temperatures probably too high for {temperature} K: "
-            f"{rotational_temperatures[rotational_temperatures >= 0.2 * temperature]}"
+            f"rotational temperatures probably too high for {temperature} K: "  # noqa: E501, G004
+            f"{rotational_temperatures[rotational_temperatures >= 0.2 * temperature]}",
         )
 
-    if not independent:
-        n = len(rotational_temperatures)
-    else:
-        n = 1.0
+    n = len(rotational_temperatures) if not independent else 1.0
     gamma = (
         np.sum(weights * n)
         - np.sum(weights * rotational_temperatures) / (3.0 * temperature)  # extra
         - np.sum(weights * rotational_temperatures**2)
         / (45.0 * temperature**2)  # extra
     )
 
     rotational_energy = constants.R * temperature * gamma / 2.0
     if not independent:
-        logger.info(f"rotational energy = {rotational_energy} J/mol")
+        logger.info(f"rotational energy = {rotational_energy} J/mol")  # noqa: G004
     return rotational_energy
 
 
-def calc_rot_entropy(
+def calc_rot_entropy(  # noqa: PLR0913
     atommasses=None,
     atomnos=None,
     atomcoords=None,
     moments=None,
     symmetry_number=1,
     environment="gas",
     method="standard",
@@ -379,59 +379,56 @@
     ...                  atommasses=data.atommasses, atomnos=data.atomnos,
     ...                  atomcoords=data.atomcoords)
     50.03250369082377
     >>> calc_rot_entropy(moments=moments, environment="water", method="garza",
     ...                  atommasses=data.atommasses, atomnos=data.atomnos,
     ...                  atomcoords=data.atomcoords)
     47.1
-    """  # noqa: E501
+    """
     temperature = np.asarray(temperature)
 
     if np.isclose(temperature, 0.0):
         logger.warning("assuming rotational entropy zero at zero temperature")
         return 0.0
 
     rotational_temperatures = _rotational_temperature(moments)
     if not rotational_temperatures.size:
         logger.warning("assuming zero rotational entropy for atomic system")
         return 0.0
 
     if not independent and np.any(rotational_temperatures >= 0.2 * temperature):
         logger.warning(
-            f"rotational temperatures probably too high for {temperature} K: "
-            f"{rotational_temperatures[rotational_temperatures >= 0.2 * temperature]}"
+            f"rotational temperatures probably too high for {temperature} K: "  # noqa: E501, G004
+            f"{rotational_temperatures[rotational_temperatures >= 0.2 * temperature]}",
         )
 
-    if not independent:
-        n = len(rotational_temperatures)
-    else:
-        n = 1.0
+    n = len(rotational_temperatures) if not independent else 1.0
     gamma = (
         np.sum(weights * n * (1.0 + np.log(temperature)))
         - np.sum(weights * np.log(rotational_temperatures))
         - 2.0 * np.log(symmetry_number)
         # The term below is an extra term that improves some linear molecules,
         # but is almost zero for most other molecules
         - np.sum(weights * rotational_temperatures**2) / (90.0 * temperature**2)
     )
-    if not independent and n > 2:
+    if not independent and n > 2:  # noqa: PLR2004
         gamma += np.log(np.pi)
 
     rotational_entropy = constants.R * gamma / 2.0
     if environment in {"gas", None} or method == "standard":
         pass
-    elif environment == "solid":  # noqa: RET506
-        raise ValueError(
-            f"environment not yet implemented: {environment}"  # noqa: EM102
+    elif environment == "solid":
+        raise ValueError(  # noqa: TRY003
+            f"environment not yet implemented: {environment}",  # noqa: EM102
         )  # noqa: RUF100
     else:
         assert atomnos is not None, "atomnos must be given"
         assert atomcoords is not None, "atomcoords must be given"
         vdw_volume = coords.get_molecular_volume(atomnos, atomcoords)
-        cav_volume, N_cav, _ = coords._garza(  # noqa: N806
+        cav_volume, N_cav, _ = coords._garza(  # noqa: N806, SLF001
             vdw_volume,
             environment,
             full_output=True,
             temperature=temperature,
             pressure=pressure,
         )
 
@@ -441,15 +438,15 @@
 
         rotational_entropy = (
             rotational_entropy
             + _sackur_tetrode(atommasses, prefactor * (r_cav - r_g) ** 3, temperature)
             - _sackur_tetrode(atommasses, prefactor * r_cav**3, temperature)
         )
     if not independent:
-        logger.info(f"rotational entropy = {rotational_entropy} J/mol·K")
+        logger.info(f"rotational entropy = {rotational_entropy} J/mol·K")  # noqa: G004
     return rotational_entropy
 
 
 def calc_vib_energy(vibfreqs=None, qrrho=True, temperature=298.15):  # noqa: FBT002
     r"""Calculate the vibrational energy of an ideal gas.
 
     This function uses equation 8-7 of Statistical Thermodynamics, McQuarrie,
@@ -502,39 +499,36 @@
 
     """  # noqa: E501
     vibrational_temperature = _vibrational_temperature(vibfreqs)
     if not vibrational_temperature.size:
         logger.warning("assuming zero vibrational energy for atomic system")
         return 0.0
 
-    if qrrho:
-        weights = _head_gordon_damping(vibfreqs)
-    else:
-        weights = 1.0
+    weights = _head_gordon_damping(vibfreqs) if qrrho else 1.0
 
     # the zero point energy (ZPE) is given below
     gamma = np.sum(weights * vibrational_temperature) / 2.0
 
     if np.isclose(temperature, 0.0):
         logger.warning("assuming zero point as vibrational energy at zero temperature")
     else:
         energy_fraction = vibrational_temperature / temperature
         gamma += np.sum(
-            weights * vibrational_temperature / (np.exp(energy_fraction) - 1.0)
+            weights * vibrational_temperature / (np.exp(energy_fraction) - 1.0),
         )
 
     vibrational_energy = constants.R * gamma
     if qrrho:
         vibrational_energy += calc_rot_energy(
             moments=_vibrational_moment(vibfreqs),
             independent=True,
             weights=1.0 - weights,
             temperature=temperature,
         )
-    logger.info(f"vibrational energy = {vibrational_energy} J/mol")
+    logger.info(f"vibrational energy = {vibrational_energy} J/mol")  # noqa: G004
     return vibrational_energy
 
 
 # TODO(schneiderfelipe): construct corrections using anharmonicity (probably
 # using corrections from a Morse potential). See also problem 6-24 of
 # Statistical Thermodynamics, McQuarrie.
 def calc_vib_entropy(vibfreqs=None, qrrho=True, temperature=298.15):  # noqa: FBT002
@@ -592,37 +586,34 @@
     # TODO(schneiderfelipe): should we use _check_vibfreqs here and remove from
     # _vibrational_temperature and _head_gordon_damping?
     vibrational_temperature = _vibrational_temperature(vibfreqs)
     if not vibrational_temperature.size:
         logger.warning("assuming zero vibrational entropy for atomic system")
         return 0.0
 
-    if qrrho:
-        weights = _head_gordon_damping(vibfreqs)
-    else:
-        weights = 1.0
+    weights = _head_gordon_damping(vibfreqs) if qrrho else 1.0
 
     energy_fraction = vibrational_temperature / temperature
     gamma = np.sum(
         weights
         * (
             energy_fraction / (np.exp(energy_fraction) - 1.0)
             - np.log(1.0 - np.exp(-energy_fraction))
-        )
+        ),
     )
 
     vibrational_entropy = constants.R * gamma
     if qrrho:
         vibrational_entropy += calc_rot_entropy(
             moments=_vibrational_moment(vibfreqs),
             independent=True,
             weights=1.0 - weights,
             temperature=temperature,
         )
-    logger.info(f"vibrational entropy = {vibrational_entropy} J/mol·K")
+    logger.info(f"vibrational entropy = {vibrational_entropy} J/mol·K")  # noqa: G004
     return vibrational_entropy
 
 
 def _sackur_tetrode(atommasses, volume, temperature=298.15):
     """Calculate the Sackur-Tetrode equation.
 
     Parameters
@@ -643,18 +634,18 @@
     >>> _sackur_tetrode(18.01528, 0.0993e-30 * constants.N_A)  # water est. free volume
     37.36
     """
     temperature = np.asarray(temperature)
 
     total_mass = np.sum(atommasses) * constants.atomic_mass
     debroglie_wavelength = constants.h / np.sqrt(
-        2.0 * np.pi * total_mass * constants.k * temperature
+        2.0 * np.pi * total_mass * constants.k * temperature,
     )
     q_trans = volume / (constants.N_A * debroglie_wavelength**3)
-    assert q_trans > 1.0, (
+    assert q_trans > 1.0, (  # noqa: PLR2004
         f"de Broglie wavelength {debroglie_wavelength} is too large for the gas to "
         "satisfy Maxwell-Boltzmann statistics (classical regime)"
     )
     return constants.R * (np.log(q_trans) + 2.5)
 
 
 def _rotational_temperature(moments=None):
@@ -672,15 +663,15 @@
     -------
     array-like
 
     Examples
     --------
     >>> i = 2.96199592e-1
     >>> _rotational_temperature()
-    array([], dtype=float64)
+    array([], ...)
     >>> _rotational_temperature(i)
     array([81.88521438])
     >>> _rotational_temperature([i])
     array([81.88521438])
     >>> _rotational_temperature([i, i])
     array([81.88521438, 81.88521438])
     >>> _rotational_temperature([0.0, i])
@@ -692,21 +683,23 @@
     >>> _rotational_temperature([i, i, i])
     array([81.88521438, 81.88521438, 81.88521438])
     """
     if moments is None:
         # assuming atomic system
         return np.array([])
     moments = np.atleast_1d(moments)
-    moments[np.abs(moments) < 1e-63] = 0  # set almost zeros to exact zeros
+    moments[
+        np.abs(moments) < 1e-63  # noqa: PLR2004
+    ] = 0  # set almost zeros to exact zeros  # noqa: PLR2004, RUF100
     moments = (
         moments[np.nonzero(moments)] * constants.atomic_mass * constants.angstrom**2
     )
 
     rotational_temperatures = constants.hbar**2 / (2.0 * constants.k * moments)
-    logger.debug(f"rotational temperatures = {rotational_temperatures} K")
+    logger.debug(f"rotational temperatures = {rotational_temperatures} K")  # noqa: G004
     return rotational_temperatures
 
 
 def _vibrational_temperature(vibfreqs=None):
     r"""Calculate vibrational temperatures.
 
     This function returns vibrational temperatures associated with all positive
@@ -722,15 +715,15 @@
     array-like
 
     Examples
     --------
     >>> vibfreq = 3374 * constants.k * constants.centi \
     ...     / (constants.h * constants.c)  # nitrogen molecule
     >>> _vibrational_temperature()
-    array([], dtype=float64)
+    array([], ...)
     >>> _vibrational_temperature(vibfreq)
     array([3374.])
     >>> _vibrational_temperature([vibfreq])
     array([3374.])
     >>> _vibrational_temperature([vibfreq, vibfreq])
     array([3374., 3374.])
 
@@ -746,15 +739,17 @@
     array([3374., 3374.])
     >>> _vibrational_temperature([vibfreq, vibfreq, vibfreq])
     array([3374., 3374., 3374.])
     """
     nu = _check_vibfreqs(vibfreqs) * constants.c / constants.centi
 
     vibrational_temperatures = constants.h * nu / constants.k
-    logger.debug(f"vibrational temperatures = {vibrational_temperatures} K")
+    logger.debug(
+        f"vibrational temperatures = {vibrational_temperatures} K",  # noqa: G004
+    )
     return vibrational_temperatures
 
 
 def _check_vibfreqs(vibfreqs=None, cutoff=-50.0):
     """Check vibrational frequencies and return them.
 
     This is mostly a helper to `_vibrational_temperature` and
@@ -781,15 +776,15 @@
     default. It is your responsability to ensure reliable values, which
     broadly means no imaginary frequency larger than this cutoff (unless we
     are dealing with transition states).
 
     Examples
     --------
     >>> _check_vibfreqs()
-    array([], dtype=float64)
+    array([], ...)
     >>> _check_vibfreqs(100.0)
     array([100.])
     >>> _check_vibfreqs([5.0, 10.0])
     array([ 5., 10.])
     >>> _check_vibfreqs([-5.0, 15.0, 100.0])
     array([  5.,  15., 100.])
     >>> _check_vibfreqs([-55.0, 15.0, 100.0])
@@ -799,15 +794,15 @@
     """
     if vibfreqs is None:
         return np.array([])
     vibfreqs = np.atleast_1d(vibfreqs)
 
     if len(vibfreqs[vibfreqs < 0]) > 0:
         logger.warning(
-            f"imaginary frequencies found: using the absolute value of all above {-cutoff}i cm-1, ignoring the rest"  # noqa: E501
+            f"imaginary frequencies found: using the absolute value of all above {-cutoff}i cm-1, ignoring the rest",  # noqa: E501, G004
         )
 
     return np.abs(vibfreqs[vibfreqs > cutoff])
 
 
 # B_av was chosen as 1.0e-44 / (atomic_mass * angstrom**2)
 def _vibrational_moment(vibfreqs=None, B_av=602.2140762081121):  # noqa: N803
@@ -831,15 +826,15 @@
     --------
     >>> _vibrational_moment(500.0)
     array([0.1059010])
     >>> _vibrational_moment(100.0)
     array([0.52913])
     >>> _vibrational_moment([5.0, 10.0])
     array([10.41,  5.250])
-    """  # noqa: E501
+    """
     # TODO(schneiderfelipe): should we receive vibrational temperatures and
     # avoid calling it twice when calling calc_vib_entropy?
 
     # I sincerely have absolutely no clue as to why we should divide by np.pi
     # and not by 2 * np.pi. The original paper says nothing about it (and the
     # equation 4 there is probably wrong), but the expression below reproduces
     # both Figure 2 of the original paper and the results returned by ORCA.
@@ -883,15 +878,15 @@
 
     >>> _head_gordon_damping([5.0, 10.0])
     array([6.e-06, 1.e-04])
     >>> _head_gordon_damping([-5.0, 5.0, 15.0, 100.0])
     array([6.e-06, 6.e-06, 4.e-04, 5.e-01])
     >>> _head_gordon_damping([-55.0, -5.0, 5.0, 15.0, 100.0])
     array([6.e-06, 6.e-06, 4.e-04, 5.e-01])
-    """  # noqa: E501
+    """
     vibfreqs = _check_vibfreqs(vibfreqs)
     return 1.0 / (1.0 + (omega / vibfreqs) ** alpha)
 
 
 def molar_volume(temperature=298.15, pressure=constants.atm):
     """Calculate the ideal gas molar volume.
 
@@ -922,9 +917,9 @@
 
     >>> molar_volume() / (constants.angstrom ** 3 * constants.N_A)
     40625.758632362515
     """
     temperature = np.asarray(temperature)
 
     molar_volume = constants.R * temperature / np.asarray(pressure)
-    logger.debug(f"molar volume = {molar_volume} Å³")
+    logger.debug(f"molar volume = {molar_volume} Å³")  # noqa: G004
     return molar_volume
```

### Comparing `overreact-1.1.0/overreact/thermo/_solv.py` & `overreact-1.2.0/overreact/thermo/_solv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python3  # noqa: EXE001
 
 """Module dedicated to the calculation of thermodynamic properties in solvation."""
 
 import logging
 
 import numpy as np
 from scipy.misc import derivative
@@ -25,15 +25,15 @@
 #    i.  doing a similar calculation as here and removing from the enthalpy or
 #    ii. by actually implementing the original method of C-PCM and excluding
 #        it from the enthalpy.
 # c. implement something closer to the original and do one of the
 #    cited in b. above.
 #
 # See doi:10.1021/cr60304a002.
-def calc_cav_entropy(
+def calc_cav_entropy(  # noqa: PLR0913
     atomnos,
     atomcoords,
     environment="water",
     temperature=298.15,
     pressure=constants.atm,
     dx=3e-5,
     order=3,
@@ -88,23 +88,27 @@
     assert atomnos is not None, "atomnos must be provided"
     assert atomcoords is not None, "atomcoords must be provided"
     vdw_volume = coords.get_molecular_volume(atomnos, atomcoords)
 
     def func(temperature, solvent):
         # TODO(schneiderfelipe): allow passing a "solvent" object everywhere so
         # that we don't repeat ourselves?
-        _, _, ratio = coords._garza(
+        _, _, ratio = coords._garza(  # noqa: SLF001
             vdw_volume,
             solvent,
             full_output=True,
             temperature=temperature,
             pressure=pressure,
         )
 
-        solvent = rx._misc._get_chemical(environment, temperature, pressure)
+        solvent = rx._misc._get_chemical(  # noqa: SLF001
+            environment,
+            temperature,
+            pressure,
+        )
 
         permittivity = solvent.permittivity
         y = 3.0 * ((permittivity - 1.0) / (permittivity + 2.0)) / (4.0 * np.pi)
         omy = 1.0 - y
         yoomy = y / omy
 
         gamma = (
@@ -117,17 +121,22 @@
             # TODO(schneiderfelipe): the following term shows up in an old
             # paper, but not in Garza's model
             + (y * solvent.Vm * pressure / (constants.R * temperature)) * ratio**3
         )
         return -constants.R * temperature * gamma
 
     cavity_entropy = derivative(
-        func, x0=temperature, dx=dx, n=1, order=order, args=(environment,)
+        func,
+        x0=temperature,
+        dx=dx,
+        n=1,
+        order=order,
+        args=(environment,),
     )
-    logger.info(f"cavity entropy = {cavity_entropy} J/mol·K")
+    logger.info(f"cavity entropy = {cavity_entropy} J/mol·K")  # noqa: G004
     return cavity_entropy
 
 
 # TODO(schneiderfelipe): the concept of free volume in polymer and membrane
 # sciences are related to the difference between the specific volume (inverse
 # of density) and the van der Waals volume (oftentimes multiplied by a factor,
 # normally 1.3), see doi:10.1007/978-3-642-40872-4_279-5. This is very similar
@@ -159,15 +168,15 @@
 # temperature/pressure, but not on the nature of the molecule. Changes in
 # solvation interaction and rotational entropy might account for the difference
 # need to validate Trouton's and Hildebrand's laws. This can be used as a
 # guide.
 #
 # The remarks above are valid for "izato". "garza" incorporates most of the
 # above in the usage of the mass density of the solvent.
-def molar_free_volume(
+def molar_free_volume(  # noqa: PLR0913
     atomnos,
     atomcoords,
     environment="water",
     method="garza",
     temperature=298.15,
     pressure=constants.atm,
 ):
@@ -246,29 +255,32 @@
     0.17
     >>> molar_free_volume(data.atomnos, data.atomcoords) \
     ...     / (constants.angstrom ** 3 * constants.N_A)
     240.
     >>> molar_free_volume(data.atomnos, data.atomcoords, environment="benzene") \
     ...     / (constants.angstrom ** 3 * constants.N_A)
     593.
-    """  # noqa: E501
+    """
     if method == "izato":
         vdw_volume, cav_volume, _ = coords.get_molecular_volume(
-            atomnos, atomcoords, method="izato", full_output=True
+            atomnos,
+            atomcoords,
+            method="izato",
+            full_output=True,
         )
         r_M, r_cav = np.cbrt(vdw_volume), np.cbrt(cav_volume)  # noqa: N806
         molar_free_volume = (r_cav - r_M) ** 3 * constants.angstrom**3 * constants.N_A
     elif method == "garza":
         # TODO(schneiderfelipe): test for the following solvents: water,
         # pentane, hexane, heptane and octane.
-        cav_volume, N_cav, _ = coords._garza(  # noqa: N806
+        cav_volume, N_cav, _ = coords._garza(  # noqa: N806, SLF001
             coords.get_molecular_volume(atomnos, atomcoords),
             environment,
             full_output=True,
             temperature=temperature,
             pressure=pressure,
         )
         molar_free_volume = N_cav * cav_volume * constants.angstrom**3 * constants.N_A
     else:
-        raise ValueError(f"unrecognized method: '{method}'")  # noqa: EM102
-    logger.debug(f"molar free volume = {molar_free_volume} Å³")
+        raise ValueError(f"unrecognized method: '{method}'")  # noqa: EM102, TRY003
+    logger.debug(f"molar free volume = {molar_free_volume} Å³")  # noqa: G004
     return molar_free_volume
```

### Comparing `overreact-1.1.0/overreact/tunnel.py` & `overreact-1.2.0/overreact/tunnel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python3  # noqa: EXE001
 
 """Module dedicated to quantum tunneling approximations."""
 
 
 from __future__ import annotations
 
 __all__ = ["eckart", "wigner"]
@@ -45,22 +45,23 @@
     2.99792458e13
     >>> _check_nu(2.0 * vibfreq) / _check_nu(vibfreq)
     2.0
     >>> _check_nu(vibfreq) == _check_nu(-vibfreq)
     True
     """
     if np.isclose(vibfreq, 0.0).any():
-        raise ValueError(
-            f"vibfreq should not be zero for tunneling: {vibfreq}"  # noqa: EM102
+        raise ValueError(  # noqa: TRY003
+            f"vibfreq should not be zero for tunneling: {vibfreq}",  # noqa: EM102
         )  # noqa: RUF100
     return np.abs(vibfreq) * constants.c / constants.centi
 
 
 def wigner(
-    vibfreq: float, temperature: Union[float, np.ndarray] = 298.15  # noqa: UP007
+    vibfreq: float,
+    temperature: Union[float, np.ndarray] = 298.15,  # noqa: UP007
 ) -> float:  # noqa: RUF100
     """Calculate the Wigner correction to quantum tunneling.
 
     Parameters
     ----------
     vibfreq : array-like
         Magnitude of the imaginary frequency in cm$^{-1}$. Only the absolute value
@@ -94,15 +95,15 @@
     """
     temperature = np.asarray(temperature)
 
     nu = _check_nu(vibfreq)
     u = constants.h * nu / (constants.k * temperature)
 
     kappa = 1.0 + (u**2) / 24.0
-    logger.info(f"Wigner tunneling coefficient: {kappa}")
+    logger.info(f"Wigner tunneling coefficient: {kappa}")  # noqa: G004
     return kappa
 
 
 def eckart(
     vibfreq: float,
     delta_forward: float,
     delta_backward: Optional[float] = None,  # noqa: UP007
@@ -163,29 +164,29 @@
     >>> eckart(190.5927, 109920.73434972763, -154.0231580734253)
     1.03525
     >>> eckart(190.5927, -154.0231580734253, 109920.73434972763)
     1.03525
     >>> eckart(190.5927, -154.0231580734253)
     1.03525
 
-    """  # noqa: E501
+    """
     temperature = np.asarray(temperature)
 
     nu = _check_nu(vibfreq)
     u = constants.h * nu / (constants.k * temperature)
 
     if delta_backward is None:
         delta_backward = delta_forward
 
-    logger.debug(f"forward  potential barrier: {delta_forward} J/mol")
-    logger.debug(f"backward potential barrier: {delta_backward} J/mol")
+    logger.debug(f"forward  potential barrier: {delta_forward} J/mol")  # noqa: G004
+    logger.debug(f"backward potential barrier: {delta_backward} J/mol")  # noqa: G004
 
     if delta_forward <= 0 or delta_backward <= 0:
         logger.warning(
-            "forward or backward barrier is non-positive, falling back to Wigner correction"  # noqa: E501
+            "forward or backward barrier is non-positive, falling back to Wigner correction",  # noqa: E501
         )
         return wigner(vibfreq, temperature)
 
     assert np.all(delta_forward > 0), "forward barrier should be positive"
     assert np.all(delta_backward > 0), "backward barrier should be positive"
 
     # convert energies in joules per mole to joules
@@ -194,21 +195,23 @@
 
     assert delta_backward is not None, "delta_backward should be given"
     two_pi = 2.0 * np.pi
     alpha1 = two_pi * delta_forward / (constants.h * nu)
     alpha2 = two_pi * delta_backward / (constants.h * nu)
 
     kappa = _eckart(u, alpha1, alpha2)
-    logger.info(f"Eckart tunneling coefficient: {kappa}")
+    logger.info(f"Eckart tunneling coefficient: {kappa}")  # noqa: G004
     return kappa
 
 
 @np.vectorize
 def _eckart(
-    u: float, alpha1: float, alpha2: Optional[float] = None  # noqa: UP007
+    u: float,
+    alpha1: float,
+    alpha2: Optional[float] = None,  # noqa: UP007
 ) -> float:  # noqa: RUF100
     """Implement of the (unsymmetrical) Eckart tunneling approximation.
 
     This is based on doi:10.1021/j100809a040 and doi:10.6028/jres.086.014.
 
     Parameters
     ----------
@@ -258,15 +261,15 @@
         alpha2 = alpha1
 
     two_pi = 2.0 * np.pi
     v1 = alpha1 * u / (two_pi)
     v2 = alpha2 * u / (two_pi)
 
     d = 4.0 * alpha1 * alpha2 - np.pi**2
-    if d > 0:
+    if d > 0:  # noqa: SIM108
         D = np.cosh(np.sqrt(d))  # noqa: N806
     else:
         D = np.cos(np.sqrt(np.abs(d)))  # noqa: N806
 
     sqrt_alpha1 = np.sqrt(alpha1)
     sqrt_alpha2 = np.sqrt(alpha2)
     F = (  # noqa: N806
```

### Comparing `overreact-1.1.0/pyproject.toml` & `overreact-1.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "overreact"
-version = "1.1.0"
+version = "1.2.0"
 description = "⚛️📈 Create and analyze chemical microkinetic models built from computational chemistry data"
 license = "MIT"
 
 authors = [
   "Felipe S. S. Schneider <schneider.felipe@posgrad.ufsc.br>",
   "Giovanni F. Caramori <giovanni.caramori@ufsc.br>",
 ]
@@ -63,28 +63,28 @@
 
 [tool.poetry.extras]
 cli = ["rich"]
 fast = ["jax", "jaxlib"]
 solvents = ["thermo"]
 
 [tool.poetry.group.dev.dependencies]
-black = { version = "^23.1a1", allow-prereleases = true }
+black = { version = "^23.3.0", extras = ["jupyter"] }
 debugpy = "^1"
-flynt = "^0.77"
+flynt = ">=0.77,<0.79"
 ipython = "^8"
 jupyter = "^1.0.0"
 matplotlib = "^3"
-mypy = "^0.991"
-pdoc = "^12"
+mypy = ">=0.991,<1.3"
+pdoc = ">=12,<14"
 perflint = "^0.7.1"
 pytest = "^7.2.0"
 pytest-cov = "^4"
-ruff = { version = "^0.0.210", allow-prereleases = true }
+ruff = { version = ">=0.0.210,<0.0.264", allow-prereleases = true }
 seaborn = "^0.12"
-types-setuptools = "^65"
+types-setuptools = ">=65,<68"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.ruff]
 target-version = "py38"
```

### Comparing `overreact-1.1.0/setup.py` & `overreact-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
  'solvents': ['thermo>=0.2,<0.3']}
 
 entry_points = \
 {'console_scripts': ['overreact = overreact._cli:main']}
 
 setup_kwargs = {
     'name': 'overreact',
-    'version': '1.1.0',
+    'version': '1.2.0',
     'description': '⚛️📈 Create and analyze chemical microkinetic models built from computational chemistry data',
-    'long_description': '--- <!-- prettier-ignore -->\n\n<div align="center">\n<p>\n<a href="https://pypi.org/project/overreact/" >\n<img src="https://img.shields.io/pypi/v/overreact" alt="PyPI" />\n</a>\n<a href="https://pypi.org/project/overreact/" >\n<img src="https://img.shields.io/pypi/pyversions/overreact" alt="Python Versions" />\n</a>\n<a href="https://github.com/geem-lab/overreact/actions/workflows/python-package.yml" />\n<img src="https://github.com/geem-lab/overreact/actions/workflows/python-package.yml/badge.svg" alt="CI" />\n</a>\n<a href="https://codecov.io/gh/geem-lab/overreact" >\n<img src="https://codecov.io/gh/geem-lab/overreact/branch/main/graph/badge.svg?token=4WAVXCRXY8" alt="Coverage" />\n</a>\n<a href="https://github.com/geem-lab/overreact/blob/main/LICENSE">\n<img src="https://img.shields.io/github/license/geem-lab/overreact" alt="License" />\n</a>\n</p>\n<p>\n<a href="https://geem-lab.github.io/overreact-guide/">\n<img src="https://img.shields.io/badge/user%20guide-available-blue" alt="User guide" />\n</a>\n<a href="https://github.com/geem-lab/overreact/discussions">\n<img src="https://img.shields.io/github/discussions/geem-lab/overreact" alt="GitHub Discussions" />\n</a>\n<a href="https://github.com/geem-lab/overreact/issues">\n<img src="https://img.shields.io/github/issues-raw/geem-lab/overreact" alt="GitHub issues" />\n</a>\n</p>\n<p>\n<a href="https://pepy.tech/project/overreact" >\n<img src="https://pepy.tech/badge/overreact/month" alt="downloads/month" />\n</a>\n<a href="https://pepy.tech/project/overreact" >\n<img src="https://pepy.tech/badge/overreact" alt="total downloads" />\n</a>\n</p>\n<p>\n<a href="https://doi.org/10.1002/jcc.26861" >\n<img src="https://img.shields.io/badge/DOI-10.1002%2Fjcc.26861-blue" alt="DOI" />\n</a>\n<a href="https://doi.org/10.5281/zenodo.7504800">\n<img src="https://zenodo.org/badge/DOI/10.5281/zenodo.7504800.svg" alt="DOI" />\n</a>\n</p>\n<p>\n<a href="https://github.com/geem-lab/overreact#funding" >\n<img src="https://img.shields.io/badge/made%20in-Brazil-009c3b" alt="Made in Brazil 🇧🇷" />\n</a>\n</p>\n</div>\n\n<div align="center">\n<img alt="overreact" src="https://raw.githubusercontent.com/geem-lab/overreact-guide/master/logo.png" />\n</div>\n\n--- <!-- prettier-ignore -->\n\n**overreact** is a **library** and a **command-line tool** for building and\nanalyzing homogeneous **microkinetic models** from **first-principles\ncalculations**:\n\n```python\nIn [1]: from overreact import api  # the api\n\nIn [2]: api.get_k("S -> E‡ -> S",  # your model\n   ...:           {"S": "data/ethane/B97-3c/staggered.out",  # your data\n   ...:            "E‡": "data/ethane/B97-3c/eclipsed.out"})\nOut[2]: array([8.16880917e+10])  # your results\n```\n\nThe user specifies a set of\nelementary reactions that are believed to be relevant for the overall chemical\nphenomena. **overreact** offers a hopefully complete but simple environment for\nhypothesis testing in first-principles chemical kinetics.\n\n<details>\n    <summary style="cursor: pointer;">\n        🤔 What is <strong>microkinetic modeling</strong>?\n    </summary>\n    <p>\n        <strong>Microkinetic modeling</strong> is a technique used to predict the outcome\n        of complex chemical reactions.\n        It can be used\n        to investigate the catalytic transformations\n        of molecules.\n        <strong>overreact</strong> makes it easy to create\n        and analyze microkinetic models built\n        from computational chemistry data.\n    </p>\n</details>\n\n<br/>\n\n<details>\n    <summary style="cursor: pointer;">\n        🧐 What do you mean by <strong>first-principles calculations</strong>?\n    </summary>\n    <p>\n        We use the term <strong>first-principles calculations</strong> to refer to\n        calculations performed using quantum chemical modern methods such as\n        <a href="https://en.wikipedia.org/wiki/Hartree%E2%80%93Fock_method">Wavefunction</a>\n        and\n        <a href="https://en.wikipedia.org/wiki/Density_functional_theory">Density Functional</a>\n        theories.\n        For instance, the three-line example code above calculates the rate of methyl rotation in ethane (at\n        <a href="https://doi.org/10.1063/1.5012601">B97-3c</a>).\n        (Rather surprisingly, the error found is less than 2%\n        <a href="http://dx.doi.org/10.1126/science.1132178">when compared to available experimental results</a>.)\n    </p>\n</details>\n\n<br/>\n\n**overreact** uses **precise thermochemical partition funtions**, **tunneling\ncorrections** and data is **parsed directly** from computational chemistry\noutput files thanks to [`cclib`](https://cclib.github.io/) (see the\n[list of its supported programs](https://cclib.github.io/#summary)).\n\n## Installation\n\n**overreact** is a Python package, so you can easily install it with\n[`pip`](https://pypi.org/project/pip/):\n\n```console\n$ pip install "overreact[cli,fast]"\n```\n\nSee the\n[installation guide](https://geem-lab.github.io/overreact-guide/install.html)\nfor more details.\n\n> **🚀** **Where to go from here?** Take a look at the\n> [short introduction](https://geem-lab.github.io/overreact-guide/tutorial.html).\n> Or see\n> [below](https://geem-lab.github.io/overreact-guide/intro.html#where-to-go-next)\n> for more guidance.\n\n## Citing **overreact**\n\nIf you use **overreact** in your research, please cite:\n\n> Schneider, F. S. S.; Caramori, G. F.\n> _**Overreact**, an in Silico Lab: Automative Quantum Chemical Microkinetic Simulations for Complex Chemical Reactions_.\n> Journal of Computational Chemistry **2022**, 44 (3), 209–217.\n> [doi:10.1002/jcc.26861](https://doi.org/10.1002/jcc.26861).\n\nHere\'s the reference in [BibTeX](http://www.bibtex.org/) format:\n\n```bibtex\n@article{overreact_paper2022,\n  title         = {Overreact, an in silico lab: Automative quantum chemical microkinetic simulations for complex chemical reactions},\n  author        = {Schneider, Felipe S. S. and Caramori, Giovanni F.},\n  year          = {2022},\n  month         = {Apr},\n  journal       = {Journal of Computational Chemistry},\n  publisher     = {Wiley},\n  volume        = {44},\n  number        = {3},\n  pages         = {209–217},\n  doi           = {10.1002/jcc.26861},\n  issn          = {1096-987x},\n  url           = {http://dx.doi.org/10.1002/jcc.26861},\n}\n@software{overreact_software2021,\n  title         = {geem-lab/overreact: v1.1.0 \\vert{} Zenodo},\n  author        = {Felipe S. S. Schneider and Let\\\'{\\i}cia M. P. Madureira and  Giovanni F. Caramori},\n  year          = {2023},\n  month         = {Jan},\n  publisher     = {Zenodo},\n  doi           = {10.5281/zenodo.7504800},\n  url           = {https://doi.org/10.5281/zenodo.7504800},\n  version       = {v1.1.0},\n  howpublished  = {\\url{https://github.com/geem-lab/overreact}},\n}\n```\n\n## License\n\n**overreact** is open-source, released under the permissive **MIT license**. See\n[the LICENSE agreement](https://github.com/geem-lab/overreact/blob/main/LICENSE).\n\n## Funding\n\nThis project was developed at the [GEEM lab](https://geem-ufsc.org/)\n([Federal University of Santa Catarina](https://en.ufsc.br/), Brazil), and was\npartially funded by the\n[Brazilian National Council for Scientific and Technological Development (CNPq)](https://cnpq.br/),\ngrant number 140485/2017-1.\n',
+    'long_description': '--- <!-- prettier-ignore -->\n\n<div align="center">\n<p>\n<a href="https://pypi.org/project/overreact/" >\n<img src="https://img.shields.io/pypi/v/overreact" alt="PyPI" />\n</a>\n<a href="https://pypi.org/project/overreact/" >\n<img src="https://img.shields.io/pypi/pyversions/overreact" alt="Python Versions" />\n</a>\n<a href="https://github.com/geem-lab/overreact/actions/workflows/python-package.yml" />\n<img src="https://github.com/geem-lab/overreact/actions/workflows/python-package.yml/badge.svg" alt="CI" />\n</a>\n<a href="https://codecov.io/gh/geem-lab/overreact" >\n<img src="https://codecov.io/gh/geem-lab/overreact/branch/main/graph/badge.svg?token=4WAVXCRXY8" alt="Coverage" />\n</a>\n<a href="https://github.com/geem-lab/overreact/blob/main/LICENSE">\n<img src="https://img.shields.io/github/license/geem-lab/overreact" alt="License" />\n</a>\n</p>\n<p>\n<a href="https://geem-lab.github.io/overreact-guide/">\n<img src="https://img.shields.io/badge/user%20guide-available-blue" alt="User guide" />\n</a>\n<a href="https://github.com/geem-lab/overreact/discussions">\n<img src="https://img.shields.io/github/discussions/geem-lab/overreact" alt="GitHub Discussions" />\n</a>\n<a href="https://github.com/geem-lab/overreact/issues">\n<img src="https://img.shields.io/github/issues-raw/geem-lab/overreact" alt="GitHub issues" />\n</a>\n</p>\n<p>\n<a href="https://pepy.tech/project/overreact" >\n<img src="https://pepy.tech/badge/overreact/month" alt="downloads/month" />\n</a>\n<a href="https://pepy.tech/project/overreact" >\n<img src="https://pepy.tech/badge/overreact" alt="total downloads" />\n</a>\n</p>\n<p>\n<a href="https://doi.org/10.1002/jcc.26861" >\n<img src="https://img.shields.io/badge/DOI-10.1002%2Fjcc.26861-blue" alt="DOI" />\n</a>\n<a href="https://doi.org/10.5281/zenodo.7504800">\n<img src="https://zenodo.org/badge/DOI/10.5281/zenodo.7504800.svg" alt="DOI" />\n</a>\n</p>\n<p>\n<a href="https://github.com/geem-lab/overreact#funding" >\n<img src="https://img.shields.io/badge/made%20in-Brazil-009c3b" alt="Made in Brazil 🇧🇷" />\n</a>\n</p>\n</div>\n\n<div align="center">\n<img alt="overreact" src="https://raw.githubusercontent.com/geem-lab/overreact-guide/master/logo.png" />\n</div>\n\n--- <!-- prettier-ignore -->\n\n**overreact** is a **library** and a **command-line tool** for building and\nanalyzing homogeneous **microkinetic models** from **first-principles\ncalculations**:\n\n```python\nIn [1]: from overreact import api  # the api\n\nIn [2]: api.get_k("S -> E‡ -> S",  # your model\n   ...:           {"S": "data/ethane/B97-3c/staggered.out",  # your data\n   ...:            "E‡": "data/ethane/B97-3c/eclipsed.out"})\nOut[2]: array([8.16880917e+10])  # your results\n```\n\nThe user specifies a set of\nelementary reactions that are believed to be relevant for the overall chemical\nphenomena. **overreact** offers a hopefully complete but simple environment for\nhypothesis testing in first-principles chemical kinetics.\n\n<details>\n    <summary style="cursor: pointer;">\n        🤔 What is <strong>microkinetic modeling</strong>?\n    </summary>\n    <p>\n        <strong>Microkinetic modeling</strong> is a technique used to predict the outcome\n        of complex chemical reactions.\n        It can be used\n        to investigate the catalytic transformations\n        of molecules.\n        <strong>overreact</strong> makes it easy to create\n        and analyze microkinetic models built\n        from computational chemistry data.\n    </p>\n</details>\n\n<br/>\n\n<details>\n    <summary style="cursor: pointer;">\n        🧐 What do you mean by <strong>first-principles calculations</strong>?\n    </summary>\n    <p>\n        We use the term <strong>first-principles calculations</strong> to refer to\n        calculations performed using quantum chemical modern methods such as\n        <a href="https://en.wikipedia.org/wiki/Hartree%E2%80%93Fock_method">Wavefunction</a>\n        and\n        <a href="https://en.wikipedia.org/wiki/Density_functional_theory">Density Functional</a>\n        theories.\n        For instance, the three-line example code above calculates the rate of methyl rotation in ethane (at\n        <a href="https://doi.org/10.1063/1.5012601">B97-3c</a>).\n        (Rather surprisingly, the error found is less than 2%\n        <a href="http://dx.doi.org/10.1126/science.1132178">when compared to available experimental results</a>.)\n    </p>\n</details>\n\n<br/>\n\n**overreact** uses **precise thermochemical partition funtions**, **tunneling\ncorrections** and data is **parsed directly** from computational chemistry\noutput files thanks to [`cclib`](https://cclib.github.io/) (see the\n[list of its supported programs](https://cclib.github.io/#summary)).\n\n## Installation\n\n**overreact** is a Python package, so you can easily install it with\n[`pip`](https://pypi.org/project/pip/):\n\n```console\n$ pip install "overreact[cli,fast]"\n```\n\nSee the\n[installation guide](https://geem-lab.github.io/overreact-guide/install.html)\nfor more details.\n\n> **🚀** **Where to go from here?** Take a look at the\n> [short introduction](https://geem-lab.github.io/overreact-guide/tutorial.html).\n> Or see\n> [below](https://geem-lab.github.io/overreact-guide/intro.html#where-to-go-next)\n> for more guidance.\n\n## Citing **overreact**\n\nIf you use **overreact** in your research, please cite:\n\n> Schneider, F. S. S.; Caramori, G. F.\n> _**Overreact**, an in Silico Lab: Automative Quantum Chemical Microkinetic Simulations for Complex Chemical Reactions_.\n> Journal of Computational Chemistry **2022**, 44 (3), 209–217.\n> [doi:10.1002/jcc.26861](https://doi.org/10.1002/jcc.26861).\n\nHere\'s the reference in [BibTeX](http://www.bibtex.org/) format:\n\n```bibtex\n@article{overreact_paper2022,\n  title         = {Overreact, an in silico lab: Automative quantum chemical microkinetic simulations for complex chemical reactions},\n  author        = {Schneider, Felipe S. S. and Caramori, Giovanni F.},\n  year          = {2022},\n  month         = {Apr},\n  journal       = {Journal of Computational Chemistry},\n  publisher     = {Wiley},\n  volume        = {44},\n  number        = {3},\n  pages         = {209–217},\n  doi           = {10.1002/jcc.26861},\n  issn          = {1096-987x},\n  url           = {http://dx.doi.org/10.1002/jcc.26861},\n}\n@software{overreact_software2021,\n  title         = {geem-lab/overreact: v1.2.0 \\vert{} Zenodo},\n  author        = {Felipe S. S. Schneider and Let\\\'{\\i}cia M. P. Madureira and  Giovanni F. Caramori},\n  year          = {2023},\n  month         = {Jan},\n  publisher     = {Zenodo},\n  doi           = {10.5281/zenodo.7504800},\n  url           = {https://doi.org/10.5281/zenodo.7504800},\n  version       = {v1.2.0},\n  howpublished  = {\\url{https://github.com/geem-lab/overreact}},\n}\n```\n\n## License\n\n**overreact** is open-source, released under the permissive **MIT license**. See\n[the LICENSE agreement](https://github.com/geem-lab/overreact/blob/main/LICENSE).\n\n## Funding\n\nThis project was developed at the [GEEM lab](https://geem-ufsc.org/)\n([Federal University of Santa Catarina](https://en.ufsc.br/), Brazil), and was\npartially funded by the\n[Brazilian National Council for Scientific and Technological Development (CNPq)](https://cnpq.br/),\ngrant number 140485/2017-1.\n',
     'author': 'Felipe S. S. Schneider',
     'author_email': 'schneider.felipe@posgrad.ufsc.br',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://geem-lab.github.io/overreact-guide/',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['overreact',
 'overreact.thermo'] package_data = \ {'': ['*']} install_requires = \
 ['cclib>=1,<2', 'scipy>=1.10,<2.0'] extras_require = \ {'cli':
 ['rich>=13,<14'], 'fast': ['jax>=0.4,<0.5', 'jaxlib>=0.4,<0.5'], 'solvents':
 ['thermo>=0.2,<0.3']} entry_points = \ {'console_scripts': ['overreact =
 overreact._cli:main']} setup_kwargs = { 'name': 'overreact', 'version':
-'1.1.0', 'description': 'âï¸ð Create and analyze chemical microkinetic
+'1.2.0', 'description': 'âï¸ð Create and analyze chemical microkinetic
 models built from computational chemistry data', 'long_description': '--- \n\n
                                       \n
 \n\n[PyPI]\n\n\n[Python_Versions]\n\n\n[CI]\n\n\n[Coverage]\n\n\n[License]\n\n
                                       \n
       \n\n[User_guide]\n\n\n[GitHub_Discussions]\n\n\n[GitHub_issues]\n\n
                                       \n
                \n\n[downloads/month]\n\n\n[total_downloads]\n\n
@@ -62,19 +62,19 @@
 www.bibtex.org/) format:\n\n```bibtex\n@article{overreact_paper2022,\n title =
 {Overreact, an in silico lab: Automative quantum chemical microkinetic
 simulations for complex chemical reactions},\n author = {Schneider, Felipe S.
 S. and Caramori, Giovanni F.},\n year = {2022},\n month = {Apr},\n journal =
 {Journal of Computational Chemistry},\n publisher = {Wiley},\n volume = {44},\n
 number = {3},\n pages = {209â217},\n doi = {10.1002/jcc.26861},\n issn =
 {1096-987x},\n url = {http://dx.doi.org/10.1002/jcc.26861},\n}\n@software
-{overreact_software2021,\n title = {geem-lab/overreact: v1.1.0 \\vert{}
+{overreact_software2021,\n title = {geem-lab/overreact: v1.2.0 \\vert{}
 Zenodo},\n author = {Felipe S. S. Schneider and Let\\\'{\\i}cia M. P. Madureira
 and Giovanni F. Caramori},\n year = {2023},\n month = {Jan},\n publisher =
 {Zenodo},\n doi = {10.5281/zenodo.7504800},\n url = {https://doi.org/10.5281/
-zenodo.7504800},\n version = {v1.1.0},\n howpublished = {\\url{https://
+zenodo.7504800},\n version = {v1.2.0},\n howpublished = {\\url{https://
 github.com/geem-lab/overreact}},\n}\n```\n\n## License\n\n**overreact** is
 open-source, released under the permissive **MIT license**. See\n[the LICENSE
 agreement](https://github.com/geem-lab/overreact/blob/main/LICENSE).\n\n##
 Funding\n\nThis project was developed at the [GEEM lab](https://geem-ufsc.org/
 )\n([Federal University of Santa Catarina](https://en.ufsc.br/), Brazil), and
 was\npartially funded by the\n[Brazilian National Council for Scientific and
 Technological Development (CNPq)](https://cnpq.br/),\ngrant number 140485/2017-
```

### Comparing `overreact-1.1.0/PKG-INFO` & `overreact-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overreact
-Version: 1.1.0
+Version: 1.2.0
 Summary: ⚛️📈 Create and analyze chemical microkinetic models built from computational chemistry data
 Home-page: https://geem-lab.github.io/overreact-guide/
 License: MIT
 Keywords: chemical-kinetics,computational-chemistry,microkinetics,reactions,thermochemistry
 Author: Felipe S. S. Schneider
 Author-email: schneider.felipe@posgrad.ufsc.br
 Requires-Python: >=3.8,<3.11
@@ -23,19 +23,19 @@
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: cli
 Provides-Extra: fast
 Provides-Extra: solvents
 Requires-Dist: cclib (>=1,<2)
-Requires-Dist: jax (>=0.4,<0.5); extra == "fast"
-Requires-Dist: jaxlib (>=0.4,<0.5); extra == "fast"
-Requires-Dist: rich (>=13,<14); extra == "cli"
+Requires-Dist: jax (>=0.4,<0.5) ; extra == "fast"
+Requires-Dist: jaxlib (>=0.4,<0.5) ; extra == "fast"
+Requires-Dist: rich (>=13,<14) ; extra == "cli"
 Requires-Dist: scipy (>=1.10,<2.0)
-Requires-Dist: thermo (>=0.2,<0.3); extra == "solvents"
+Requires-Dist: thermo (>=0.2,<0.3) ; extra == "solvents"
 Project-URL: API documentation, https://geem-lab.github.io/overreact/
 Project-URL: Bug Tracker, https://github.com/geem-lab/overreact/issues
 Project-URL: Citation, https://doi.org/10.1002/jcc.26861
 Project-URL: Documentation, https://geem-lab.github.io/overreact-guide/
 Project-URL: Discussions, https://github.com/geem-lab/overreact/discussions
 Project-URL: PyPI, https://pypi.org/project/overreact/
 Project-URL: Repository, https://github.com/geem-lab/overreact
@@ -204,22 +204,22 @@
   number        = {3},
   pages         = {209–217},
   doi           = {10.1002/jcc.26861},
   issn          = {1096-987x},
   url           = {http://dx.doi.org/10.1002/jcc.26861},
 }
 @software{overreact_software2021,
-  title         = {geem-lab/overreact: v1.1.0 \vert{} Zenodo},
+  title         = {geem-lab/overreact: v1.2.0 \vert{} Zenodo},
   author        = {Felipe S. S. Schneider and Let\'{\i}cia M. P. Madureira and  Giovanni F. Caramori},
   year          = {2023},
   month         = {Jan},
   publisher     = {Zenodo},
   doi           = {10.5281/zenodo.7504800},
   url           = {https://doi.org/10.5281/zenodo.7504800},
-  version       = {v1.1.0},
+  version       = {v1.2.0},
   howpublished  = {\url{https://github.com/geem-lab/overreact}},
 }
 ```
 
 ## License
 
 **overreact** is open-source, released under the permissive **MIT license**. See
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: overreact Version: 1.1.0 Summary: âï¸ð Create
+Metadata-Version: 2.1 Name: overreact Version: 1.2.0 Summary: âï¸ð Create
 and analyze chemical microkinetic models built from computational chemistry
 data Home-page: https://geem-lab.github.io/overreact-guide/ License: MIT
 Keywords: chemical-kinetics,computational-
 chemistry,microkinetics,reactions,thermochemistry Author: Felipe S. S.
 Schneider Author-email: schneider.felipe@posgrad.ufsc.br Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 4 - Beta Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
@@ -11,18 +11,18 @@
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Topic :: Education Classifier: Topic :: Scientific/Engineering :: Atmospheric
 Science Classifier: Topic :: Scientific/Engineering :: Chemistry Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Provides-Extra:
 cli Provides-Extra: fast Provides-Extra: solvents Requires-Dist: cclib (>=1,<2)
-Requires-Dist: jax (>=0.4,<0.5); extra == "fast" Requires-Dist: jaxlib
-(>=0.4,<0.5); extra == "fast" Requires-Dist: rich (>=13,<14); extra == "cli"
-Requires-Dist: scipy (>=1.10,<2.0) Requires-Dist: thermo (>=0.2,<0.3); extra ==
-"solvents" Project-URL: API documentation, https://geem-lab.github.io/
+Requires-Dist: jax (>=0.4,<0.5) ; extra == "fast" Requires-Dist: jaxlib
+(>=0.4,<0.5) ; extra == "fast" Requires-Dist: rich (>=13,<14) ; extra == "cli"
+Requires-Dist: scipy (>=1.10,<2.0) Requires-Dist: thermo (>=0.2,<0.3) ; extra
+== "solvents" Project-URL: API documentation, https://geem-lab.github.io/
 overreact/ Project-URL: Bug Tracker, https://github.com/geem-lab/overreact/
 issues Project-URL: Citation, https://doi.org/10.1002/jcc.26861 Project-URL:
 Documentation, https://geem-lab.github.io/overreact-guide/ Project-URL:
 Discussions, https://github.com/geem-lab/overreact/discussions Project-URL:
 PyPI, https://pypi.org/project/overreact/ Project-URL: Repository, https://
 github.com/geem-lab/overreact Description-Content-Type: text/markdown ---
               [PyPI] [Python_Versions] [CI] [Coverage] [License]
@@ -73,18 +73,18 @@
 www.bibtex.org/) format: ```bibtex @article{overreact_paper2022, title =
 {Overreact, an in silico lab: Automative quantum chemical microkinetic
 simulations for complex chemical reactions}, author = {Schneider, Felipe S. S.
 and Caramori, Giovanni F.}, year = {2022}, month = {Apr}, journal = {Journal of
 Computational Chemistry}, publisher = {Wiley}, volume = {44}, number = {3},
 pages = {209â217}, doi = {10.1002/jcc.26861}, issn = {1096-987x}, url =
 {http://dx.doi.org/10.1002/jcc.26861}, } @software{overreact_software2021,
-title = {geem-lab/overreact: v1.1.0 \vert{} Zenodo}, author = {Felipe S. S.
+title = {geem-lab/overreact: v1.2.0 \vert{} Zenodo}, author = {Felipe S. S.
 Schneider and Let\'{\i}cia M. P. Madureira and Giovanni F. Caramori}, year =
 {2023}, month = {Jan}, publisher = {Zenodo}, doi = {10.5281/zenodo.7504800},
-url = {https://doi.org/10.5281/zenodo.7504800}, version = {v1.1.0},
+url = {https://doi.org/10.5281/zenodo.7504800}, version = {v1.2.0},
 howpublished = {\url{https://github.com/geem-lab/overreact}}, } ``` ## License
 **overreact** is open-source, released under the permissive **MIT license**.
 See [the LICENSE agreement](https://github.com/geem-lab/overreact/blob/main/
 LICENSE). ## Funding This project was developed at the [GEEM lab](https://geem-
 ufsc.org/) ([Federal University of Santa Catarina](https://en.ufsc.br/),
 Brazil), and was partially funded by the [Brazilian National Council for
 Scientific and Technological Development (CNPq)](https://cnpq.br/), grant
```

