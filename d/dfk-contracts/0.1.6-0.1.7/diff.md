# Comparing `tmp/dfk_contracts-0.1.6.tar.gz` & `tmp/dfk_contracts-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfk_contracts-0.1.6.tar", max compression
+gzip compressed data, was "dfk_contracts-0.1.7.tar", max compression
```

## Comparing `dfk_contracts-0.1.6.tar` & `dfk_contracts-0.1.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0   584106 2023-04-20 16:46:33.470587 dfk_contracts-0.1.6/dfk_contracts/DFK_ABIS.json
--rw-r--r--   0        0        0     6165 2023-04-20 16:46:33.331337 dfk_contracts-0.1.6/dfk_contracts/abi_contract_wrapper.py
--rw-r--r--   0        0        0     1285 2023-04-20 16:46:33.332783 dfk_contracts-0.1.6/dfk_contracts/abi_multi_contract_wrapper.py
--rw-r--r--   0        0        0     5782 2023-04-20 16:46:33.470192 dfk_contracts-0.1.6/dfk_contracts/all_dfk_contracts.py
--rw-r--r--   0        0        0     6443 2023-04-20 16:46:33.340389 dfk_contracts-0.1.6/dfk_contracts/contracts/airdrop_claim.py
--rw-r--r--   0        0        0     7938 2023-04-20 16:46:33.344692 dfk_contracts-0.1.6/dfk_contracts/contracts/alchemist.py
--rw-r--r--   0        0        0    11346 2023-04-20 16:46:33.348522 dfk_contracts-0.1.6/dfk_contracts/contracts/assisting_auction.py
--rw-r--r--   0        0        0    28633 2023-04-20 16:46:33.352611 dfk_contracts-0.1.6/dfk_contracts/contracts/atonement_crystal.py
--rw-r--r--   0        0        0     5368 2023-04-20 16:46:33.354351 dfk_contracts-0.1.6/dfk_contracts/contracts/banker.py
--rw-r--r--   0        0        0     9787 2023-04-20 16:46:33.356980 dfk_contracts-0.1.6/dfk_contracts/contracts/birthday_cake.py
--rw-r--r--   0        0        0     8977 2023-04-20 16:46:33.359385 dfk_contracts-0.1.6/dfk_contracts/contracts/charity_fund.py
--rw-r--r--   0        0        0    13451 2023-04-20 16:46:33.362195 dfk_contracts-0.1.6/dfk_contracts/contracts/crystal_core.py
--rw-r--r--   0        0        0    25794 2023-04-20 16:46:33.370883 dfk_contracts-0.1.6/dfk_contracts/contracts/dark_summoning.py
--rw-r--r--   0        0        0    55830 2023-04-20 16:46:33.378548 dfk_contracts-0.1.6/dfk_contracts/contracts/dfk_duel_s2.py
--rw-r--r--   0        0        0    14296 2023-04-20 16:46:33.380876 dfk_contracts-0.1.6/dfk_contracts/contracts/duel_rank_claim.py
--rw-r--r--   0        0        0     8728 2023-04-20 16:46:33.382521 dfk_contracts-0.1.6/dfk_contracts/contracts/erc20.py
--rw-r--r--   0        0        0     5901 2023-04-20 16:46:33.383672 dfk_contracts-0.1.6/dfk_contracts/contracts/flag_storage_v2.py
--rw-r--r--   0        0        0     7483 2023-04-20 16:46:33.384912 dfk_contracts-0.1.6/dfk_contracts/contracts/gen0_airdrop.py
--rw-r--r--   0        0        0    25083 2023-04-20 16:46:33.386922 dfk_contracts-0.1.6/dfk_contracts/contracts/gen0_reroll.py
--rw-r--r--   0        0        0    40923 2023-04-20 16:46:33.388869 dfk_contracts-0.1.6/dfk_contracts/contracts/gene_reroll.py
--rw-r--r--   0        0        0    16211 2023-04-20 16:46:33.391435 dfk_contracts-0.1.6/dfk_contracts/contracts/hero_auction.py
--rw-r--r--   0        0        0    10449 2023-04-20 16:46:33.393291 dfk_contracts-0.1.6/dfk_contracts/contracts/hero_bridge.py
--rw-r--r--   0        0        0    30987 2023-04-20 16:46:33.401862 dfk_contracts-0.1.6/dfk_contracts/contracts/hero_core.py
--rw-r--r--   0        0        0    28714 2023-04-20 16:46:33.405713 dfk_contracts-0.1.6/dfk_contracts/contracts/hero_summoning.py
--rw-r--r--   0        0        0    24467 2023-04-20 16:46:33.409796 dfk_contracts-0.1.6/dfk_contracts/contracts/item_bridge.py
--rw-r--r--   0        0        0    12535 2023-04-20 16:46:33.410594 dfk_contracts-0.1.6/dfk_contracts/contracts/item_consumer.py
--rw-r--r--   0        0        0    11557 2023-04-20 16:46:33.412092 dfk_contracts-0.1.6/dfk_contracts/contracts/item_gold_trader_v2.py
--rw-r--r--   0        0        0    26862 2023-04-20 16:46:33.416170 dfk_contracts-0.1.6/dfk_contracts/contracts/jewel_token.py
--rw-r--r--   0        0        0    15192 2023-04-20 16:46:33.418435 dfk_contracts-0.1.6/dfk_contracts/contracts/land_auction.py
--rw-r--r--   0        0        0    18105 2023-04-20 16:46:33.420950 dfk_contracts-0.1.6/dfk_contracts/contracts/land_core.py
--rw-r--r--   0        0        0    30381 2023-04-20 16:46:33.425186 dfk_contracts-0.1.6/dfk_contracts/contracts/master_gardener.py
--rw-r--r--   0        0        0    25321 2023-04-20 16:46:33.427296 dfk_contracts-0.1.6/dfk_contracts/contracts/meditation_circle.py
--rw-r--r--   0        0        0     9664 2023-04-20 16:46:33.428542 dfk_contracts-0.1.6/dfk_contracts/contracts/multicall3.py
--rw-r--r--   0        0        0     7278 2023-04-20 16:46:33.429480 dfk_contracts-0.1.6/dfk_contracts/contracts/pasture.py
--rw-r--r--   0        0        0    15191 2023-04-20 16:46:33.431774 dfk_contracts-0.1.6/dfk_contracts/contracts/pet_auction.py
--rw-r--r--   0        0        0     9508 2023-04-20 16:46:33.433482 dfk_contracts-0.1.6/dfk_contracts/contracts/pet_bridge.py
--rw-r--r--   0        0        0    20801 2023-04-20 16:46:33.440079 dfk_contracts-0.1.6/dfk_contracts/contracts/pet_core.py
--rw-r--r--   0        0        0     9676 2023-04-20 16:46:33.441798 dfk_contracts-0.1.6/dfk_contracts/contracts/pet_exchange.py
--rw-r--r--   0        0        0    19016 2023-04-20 16:46:33.444778 dfk_contracts-0.1.6/dfk_contracts/contracts/pet_hatching.py
--rw-r--r--   0        0        0    20106 2023-04-20 16:46:33.366801 dfk_contracts-0.1.6/dfk_contracts/contracts/power_token.py
--rw-r--r--   0        0        0    33463 2023-04-20 16:46:33.448757 dfk_contracts-0.1.6/dfk_contracts/contracts/power_up_manager.py
--rw-r--r--   0        0        0    14471 2023-04-20 16:46:33.450982 dfk_contracts-0.1.6/dfk_contracts/contracts/profiles.py
--rw-r--r--   0        0        0    20908 2023-04-20 16:46:33.453862 dfk_contracts-0.1.6/dfk_contracts/contracts/quest_core.py
--rw-r--r--   0        0        0    23204 2023-04-20 16:46:33.457090 dfk_contracts-0.1.6/dfk_contracts/contracts/raffle_master.py
--rw-r--r--   0        0        0     9787 2023-04-20 16:46:33.458656 dfk_contracts-0.1.6/dfk_contracts/contracts/raffle_ticket.py
--rw-r--r--   0        0        0     9147 2023-04-20 16:46:33.460218 dfk_contracts-0.1.6/dfk_contracts/contracts/stone_carver.py
--rw-r--r--   0        0        0     6206 2023-04-20 16:46:33.461272 dfk_contracts-0.1.6/dfk_contracts/contracts/stylist.py
--rw-r--r--   0        0        0     7897 2023-04-20 16:46:33.462407 dfk_contracts-0.1.6/dfk_contracts/contracts/token_disburse.py
--rw-r--r--   0        0        0     4541 2023-04-20 16:46:33.463269 dfk_contracts-0.1.6/dfk_contracts/contracts/uniswap_v2_factory.py
--rw-r--r--   0        0        0    21550 2023-04-20 16:46:33.467047 dfk_contracts-0.1.6/dfk_contracts/contracts/uniswap_v2_router.py
--rw-r--r--   0        0        0    18537 2023-04-20 16:46:33.469549 dfk_contracts-0.1.6/dfk_contracts/contracts/validator_fund.py
--rw-r--r--   0        0        0     2008 2023-04-20 16:46:33.329270 dfk_contracts-0.1.6/dfk_contracts/credentials.py
--rw-r--r--   0        0        0      779 2023-04-20 16:46:33.326875 dfk_contracts-0.1.6/dfk_contracts/solidity_types.py
--rw-r--r--   0        0        0      365 2023-04-21 15:18:44.353200 dfk_contracts-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 dfk_contracts-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0   583935 2023-04-25 22:06:58.181848 dfk_contracts-0.1.7/dfk_contracts/DFK_ABIS.json
+-rw-r--r--   0        0        0     6293 2023-04-25 22:06:58.025972 dfk_contracts-0.1.7/dfk_contracts/abi_contract_wrapper.py
+-rw-r--r--   0        0        0     1287 2023-04-25 22:06:58.026403 dfk_contracts-0.1.7/dfk_contracts/abi_multi_contract_wrapper.py
+-rw-r--r--   0        0        0     5782 2023-04-25 22:06:58.181367 dfk_contracts-0.1.7/dfk_contracts/all_dfk_contracts.py
+-rw-r--r--   0        0        0     6443 2023-04-25 22:06:58.028565 dfk_contracts-0.1.7/dfk_contracts/contracts/airdrop_claim.py
+-rw-r--r--   0        0        0     7938 2023-04-25 22:06:58.029747 dfk_contracts-0.1.7/dfk_contracts/contracts/alchemist.py
+-rw-r--r--   0        0        0    11346 2023-04-25 22:06:58.031423 dfk_contracts-0.1.7/dfk_contracts/contracts/assisting_auction.py
+-rw-r--r--   0        0        0    28633 2023-04-25 22:06:58.033746 dfk_contracts-0.1.7/dfk_contracts/contracts/atonement_crystal.py
+-rw-r--r--   0        0        0     5368 2023-04-25 22:06:58.034779 dfk_contracts-0.1.7/dfk_contracts/contracts/banker.py
+-rw-r--r--   0        0        0     9787 2023-04-25 22:06:58.037426 dfk_contracts-0.1.7/dfk_contracts/contracts/birthday_cake.py
+-rw-r--r--   0        0        0     8977 2023-04-25 22:06:58.039106 dfk_contracts-0.1.7/dfk_contracts/contracts/charity_fund.py
+-rw-r--r--   0        0        0    13451 2023-04-25 22:06:58.041901 dfk_contracts-0.1.7/dfk_contracts/contracts/crystal_core.py
+-rw-r--r--   0        0        0    25794 2023-04-25 22:06:58.048092 dfk_contracts-0.1.7/dfk_contracts/contracts/dark_summoning.py
+-rw-r--r--   0        0        0    55830 2023-04-25 22:06:58.053684 dfk_contracts-0.1.7/dfk_contracts/contracts/dfk_duel_s2.py
+-rw-r--r--   0        0        0    14296 2023-04-25 22:06:58.055475 dfk_contracts-0.1.7/dfk_contracts/contracts/duel_rank_claim.py
+-rw-r--r--   0        0        0     8728 2023-04-25 22:06:58.056639 dfk_contracts-0.1.7/dfk_contracts/contracts/erc20.py
+-rw-r--r--   0        0        0     5901 2023-04-25 22:06:58.057454 dfk_contracts-0.1.7/dfk_contracts/contracts/flag_storage_v2.py
+-rw-r--r--   0        0        0     7483 2023-04-25 22:06:58.058333 dfk_contracts-0.1.7/dfk_contracts/contracts/gen0_airdrop.py
+-rw-r--r--   0        0        0    25083 2023-04-25 22:06:58.059950 dfk_contracts-0.1.7/dfk_contracts/contracts/gen0_reroll.py
+-rw-r--r--   0        0        0    40923 2023-04-25 22:06:58.062085 dfk_contracts-0.1.7/dfk_contracts/contracts/gene_reroll.py
+-rw-r--r--   0        0        0    16211 2023-04-25 22:06:58.064385 dfk_contracts-0.1.7/dfk_contracts/contracts/hero_auction.py
+-rw-r--r--   0        0        0    10449 2023-04-25 22:06:58.066014 dfk_contracts-0.1.7/dfk_contracts/contracts/hero_bridge.py
+-rw-r--r--   0        0        0    30987 2023-04-25 22:06:58.069135 dfk_contracts-0.1.7/dfk_contracts/contracts/hero_core.py
+-rw-r--r--   0        0        0    28714 2023-04-25 22:06:58.073298 dfk_contracts-0.1.7/dfk_contracts/contracts/hero_summoning.py
+-rw-r--r--   0        0        0    24467 2023-04-25 22:06:58.081452 dfk_contracts-0.1.7/dfk_contracts/contracts/item_bridge.py
+-rw-r--r--   0        0        0    12535 2023-04-25 22:06:58.082479 dfk_contracts-0.1.7/dfk_contracts/contracts/item_consumer.py
+-rw-r--r--   0        0        0    11398 2023-04-25 22:06:58.084529 dfk_contracts-0.1.7/dfk_contracts/contracts/item_gold_trader_v2.py
+-rw-r--r--   0        0        0    26862 2023-04-25 22:06:58.093235 dfk_contracts-0.1.7/dfk_contracts/contracts/jewel_token.py
+-rw-r--r--   0        0        0    15192 2023-04-25 22:06:58.099049 dfk_contracts-0.1.7/dfk_contracts/contracts/land_auction.py
+-rw-r--r--   0        0        0    18105 2023-04-25 22:06:58.101803 dfk_contracts-0.1.7/dfk_contracts/contracts/land_core.py
+-rw-r--r--   0        0        0    30381 2023-04-25 22:06:58.108507 dfk_contracts-0.1.7/dfk_contracts/contracts/master_gardener.py
+-rw-r--r--   0        0        0    25321 2023-04-25 22:06:58.110926 dfk_contracts-0.1.7/dfk_contracts/contracts/meditation_circle.py
+-rw-r--r--   0        0        0     9664 2023-04-25 22:06:58.112245 dfk_contracts-0.1.7/dfk_contracts/contracts/multicall3.py
+-rw-r--r--   0        0        0     7278 2023-04-25 22:06:58.113228 dfk_contracts-0.1.7/dfk_contracts/contracts/pasture.py
+-rw-r--r--   0        0        0    15191 2023-04-25 22:06:58.115583 dfk_contracts-0.1.7/dfk_contracts/contracts/pet_auction.py
+-rw-r--r--   0        0        0     9508 2023-04-25 22:06:58.117563 dfk_contracts-0.1.7/dfk_contracts/contracts/pet_bridge.py
+-rw-r--r--   0        0        0    20801 2023-04-25 22:06:58.119962 dfk_contracts-0.1.7/dfk_contracts/contracts/pet_core.py
+-rw-r--r--   0        0        0     9676 2023-04-25 22:06:58.121449 dfk_contracts-0.1.7/dfk_contracts/contracts/pet_exchange.py
+-rw-r--r--   0        0        0    19016 2023-04-25 22:06:58.125365 dfk_contracts-0.1.7/dfk_contracts/contracts/pet_hatching.py
+-rw-r--r--   0        0        0    20106 2023-04-25 22:06:58.045256 dfk_contracts-0.1.7/dfk_contracts/contracts/power_token.py
+-rw-r--r--   0        0        0    33463 2023-04-25 22:06:58.130246 dfk_contracts-0.1.7/dfk_contracts/contracts/power_up_manager.py
+-rw-r--r--   0        0        0    14471 2023-04-25 22:06:58.133668 dfk_contracts-0.1.7/dfk_contracts/contracts/profiles.py
+-rw-r--r--   0        0        0    20908 2023-04-25 22:06:58.137415 dfk_contracts-0.1.7/dfk_contracts/contracts/quest_core.py
+-rw-r--r--   0        0        0    23204 2023-04-25 22:06:58.142928 dfk_contracts-0.1.7/dfk_contracts/contracts/raffle_master.py
+-rw-r--r--   0        0        0     9787 2023-04-25 22:06:58.144684 dfk_contracts-0.1.7/dfk_contracts/contracts/raffle_ticket.py
+-rw-r--r--   0        0        0     9147 2023-04-25 22:06:58.147117 dfk_contracts-0.1.7/dfk_contracts/contracts/stone_carver.py
+-rw-r--r--   0        0        0     6206 2023-04-25 22:06:58.149028 dfk_contracts-0.1.7/dfk_contracts/contracts/stylist.py
+-rw-r--r--   0        0        0     7897 2023-04-25 22:06:58.156596 dfk_contracts-0.1.7/dfk_contracts/contracts/token_disburse.py
+-rw-r--r--   0        0        0     4541 2023-04-25 22:06:58.159167 dfk_contracts-0.1.7/dfk_contracts/contracts/uniswap_v2_factory.py
+-rw-r--r--   0        0        0    21550 2023-04-25 22:06:58.166525 dfk_contracts-0.1.7/dfk_contracts/contracts/uniswap_v2_router.py
+-rw-r--r--   0        0        0    18537 2023-04-25 22:06:58.180470 dfk_contracts-0.1.7/dfk_contracts/contracts/validator_fund.py
+-rw-r--r--   0        0        0     2008 2023-04-25 22:06:58.025029 dfk_contracts-0.1.7/dfk_contracts/credentials.py
+-rw-r--r--   0        0        0      819 2023-04-25 22:06:58.024682 dfk_contracts-0.1.7/dfk_contracts/solidity_types.py
+-rw-r--r--   0        0        0      364 2023-04-25 22:07:42.044236 dfk_contracts-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 dfk_contracts-0.1.7/PKG-INFO
```

### Comparing `dfk_contracts-0.1.6/dfk_contracts/DFK_ABIS.json` & `dfk_contracts-0.1.7/dfk_contracts/DFK_ABIS.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999683383991895%*

 * *Differences: {"'CONTRACTS'": "{'ItemGoldTraderV2': {'ABI': {delete: [0]}}}"}*

```diff
@@ -22349,27 +22349,14 @@
         },
         "ItemGoldTraderV2": {
             "ABI": [
                 {
                     "anonymous": false,
                     "inputs": [
                         {
-                            "indexed": false,
-                            "internalType": "uint8",
-                            "name": "version",
-                            "type": "uint8"
-                        }
-                    ],
-                    "name": "Initialized",
-                    "type": "event"
-                },
-                {
-                    "anonymous": false,
-                    "inputs": [
-                        {
                             "indexed": true,
                             "internalType": "address",
                             "name": "item",
                             "type": "address"
                         },
                         {
                             "indexed": false,
```

### Comparing `dfk_contracts-0.1.6/dfk_contracts/abi_contract_wrapper.py` & `dfk_contracts-0.1.7/dfk_contracts/abi_contract_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #! /usr/bin/env python
 from web3 import Web3
 from web3.middleware.geth_poa import geth_poa_middleware
 from web3.logs import DISCARD
 
 from .credentials import Credentials
 
-from .solidity_types import *
-from web3.contract import Contract
-from typing import Dict, Tuple, Union, Optional, Any
+from .solidity_types import (address, ChecksumAddress, TxReceipt, AttributeDict)
+from web3.contract.contract import Contract
+from typing import Dict, Tuple, Union, Optional, Any, Sequence
 
 DEFAULT_TIMEOUT = 30
 DEFAULT_MAX_GAS = 50
 DEFAULT_MAX_PRIORITY_GAS = 3
 
 W3_INSTANCES: Dict[str, Web3] = {}
 
@@ -33,18 +33,18 @@
         global W3_INSTANCES
         w3 = W3_INSTANCES.get(self.rpc, None)
         if not w3:
             w3 = Web3(Web3.HTTPProvider(self.rpc))
             w3.middleware_onion.inject(geth_poa_middleware, layer=0)
             W3_INSTANCES[self.rpc] = w3
         self.w3 = w3
-        self.contract_address:HexAddress = self.w3.toChecksumAddress(contract_address)
+        self.contract_address:ChecksumAddress = self.w3.to_checksum_address(contract_address)
 
-        self.max_gas_wei = self.w3.toWei(max_gas_gwei, 'gwei')
-        self.max_priority_wei = self.w3.toWei(max_priority_gwei, 'gwei')
+        self.max_gas_wei = self.w3.to_wei(max_gas_gwei, 'gwei')
+        self.max_priority_wei = self.w3.to_wei(max_priority_gwei, 'gwei')
 
         self.contract = self.w3.eth.contract(self.contract_address, abi=self.abi)
 
     def get_nonce_and_update(self, address:address, force_fetch=True) -> int:
         # FIXME: I think there's a bug in the caching logic below that lets
         # nonces run ahead of where they should be and causes transactions to
         # fail.
@@ -52,15 +52,15 @@
         # every transaction
         # - Athiriyya 13 December 2022
 
         # We keep track of our own nonce, and only re-fetch it if a 'nonce too low'
         # error gets thrown       
         nonce = self.nonces.get(address, 0) 
         if force_fetch or nonce == 0:
-            nonce = self.w3.eth.getTransactionCount( address, 'pending')
+            nonce = self.w3.eth.get_transaction_count( address, 'pending')
 
         # Store the next nonce this address will use, and return the current one
         self.nonces[address] = nonce + 1
         return nonce
 
     def get_gas_dict_and_update(self, address:address) -> Dict[str, int]:
         nonce = self.get_nonce_and_update(address)
@@ -84,20 +84,20 @@
             }
         return gas_dict
 
     def call_contract_function(self, function_name:str, *args) -> Any:
         contract_func = getattr(self.contract, function_name)
         return contract_func(*args).call()
 
-    def get_custom_contract(self, contract_address:HexAddress, abi:str | None=None) -> Contract:
+    def get_custom_contract(self, contract_address:ChecksumAddress, abi:str | None=None) -> Contract:
         # TODO: Many custom contracts for e.g. ERC20 tokens could
         # be re-used by caching a contracts dictionary keyed by address
         # For now, just return a new contract
         abi = abi or self.abi
-        checked_addr = self.w3.toChecksumAddress(contract_address)
+        checked_addr = self.w3.to_checksum_address(contract_address)
         contract = self.w3.eth.contract(checked_addr, abi=abi)
         return contract
 
     def send_transaction(self,
                          tx,
                          cred:Credentials,
                          extra_dict:Dict[str,Any] | None = None
@@ -105,15 +105,15 @@
         # Some transactions require extra information or fees when building 
         # the transaction. e.g. bridging functions need a {'value': <bridge_fee_in_wei>}
         # argument. If supplied, add that extra info
         address = cred.address  
         gas_dict = self.get_gas_dict_and_update(address)
         if extra_dict:
             gas_dict.update(extra_dict)
-        tx_dict = tx.buildTransaction(gas_dict)    
+        tx_dict = tx.build_transaction(gas_dict)    
         signed_tx = self.w3.eth.account.sign_transaction(tx_dict, private_key=cred.private_key)
         try:
             self.w3.eth.send_raw_transaction(signed_tx.rawTransaction)
 
         except Exception as e:
             if 'nonce too low' in str(e):
                 nonce = self.get_nonce_and_update(address, force_fetch=True)
@@ -127,27 +127,27 @@
             timeout=self.timeout,
         )
         return receipt
 
     def get_legacy_gas_fee(self) ->Tuple[int, int]:
         # See: https://web3py.readthedocs.io/en/stable/gas_price.html#gas-price-api
         # Some transactions may require a gas dict with the keys {'gasPrice': x_wei, '': y_wei}
-        block = self.w3.eth.getBlock("pending")
-        base_gas = block.gasUsed + self.w3.toWei(50, 'gwei')
-        gas_limit =block.gasLimit
+        block = self.w3.eth.get_block("pending")
+        base_gas = block.get('gasUsed', 2_500_000) + self.w3.to_wei(50, 'gwei')
+        gas_limit =block.get('gasLimit', 2_500_000)
 
         return base_gas, gas_limit
 
     def tx_receipt_for_hash(self, tx_hash:address) -> TxReceipt:
         tx_receipt = self.w3.eth.get_transaction_receipt(tx_hash)
         return tx_receipt
 
     def parse_events(self, tx_receipt:TxReceipt, event_names:Sequence[str] | None = None) -> Dict[str, AttributeDict]:
         event_dicts = {}
         for event in self.contract.events: # type: ignore
-            eds = event().processReceipt(tx_receipt, errors=DISCARD)
+            eds = event().process_receipt(tx_receipt, errors=DISCARD)
             if eds:
                 for ed in eds:
                     event_dicts.setdefault(ed.event,[]).append(ed)
         if event_names:
             event_dicts = {k:v for k,v in event_dicts.items() if k in event_names}
         return event_dicts
```

### Comparing `dfk_contracts-0.1.6/dfk_contracts/abi_multi_contract_wrapper.py` & `dfk_contracts-0.1.7/dfk_contracts/abi_multi_contract_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,9 +30,9 @@
         w3 = W3_INSTANCES.get(self.rpc, None)
         if not w3:
             w3 = Web3(Web3.HTTPProvider(self.rpc))
             w3.middleware_onion.inject(geth_poa_middleware, layer=0)
             W3_INSTANCES[self.rpc] = w3
         self.w3 = w3
 
-        self.max_gas_wei = self.w3.toWei(max_gas_gwei, 'gwei')
-        self.max_priority_wei = self.w3.toWei(max_priority_gwei, 'gwei')
+        self.max_gas_wei = self.w3.to_wei(max_gas_gwei, 'gwei')
+        self.max_priority_wei = self.w3.to_wei(max_priority_gwei, 'gwei')
```

### Comparing `dfk_contracts-0.1.6/dfk_contracts/all_dfk_contracts.py` & `dfk_contracts-0.1.7/dfk_contracts/all_dfk_contracts.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/airdrop_claim.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/airdrop_claim.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/alchemist.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/alchemist.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/assisting_auction.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/assisting_auction.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/atonement_crystal.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/atonement_crystal.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/banker.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/banker.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/birthday_cake.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/birthday_cake.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/charity_fund.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/charity_fund.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/crystal_core.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/crystal_core.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/dark_summoning.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/dark_summoning.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/dfk_duel_s2.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/dfk_duel_s2.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/duel_rank_claim.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/duel_rank_claim.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/erc20.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/erc20.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/flag_storage_v2.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/flag_storage_v2.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/gen0_airdrop.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/gen0_airdrop.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/gen0_reroll.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/gen0_reroll.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/gene_reroll.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/gene_reroll.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/hero_auction.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/hero_auction.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/hero_bridge.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/hero_bridge.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/hero_core.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/hero_core.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/hero_summoning.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/hero_summoning.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/item_bridge.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/item_bridge.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/item_consumer.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/item_consumer.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/item_gold_trader_v2.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/item_gold_trader_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 CONTRACT_ADDRESS =     {
     "cv": "0x0f85fdf6c561C42d6b46d0E27ea6Aa9Bf9476B3f",
     "sd": "0x3Eab8a8F71dDA3e6c907C74302B734805C4f3278"
 }
 
 ABI = """[
-    {"name": "Initialized", "type": "event", "inputs": [{"name": "version", "type": "uint8", "internalType": "uint8", "indexed": false}], "anonymous": false},
     {"name": "ItemAdded", "type": "event", "inputs": [{"name": "item", "type": "address", "internalType": "address", "indexed": true}, {"name": "startingPrice", "type": "uint256", "internalType": "uint256", "indexed": false}, {"name": "playerSellPrice", "type": "uint256", "internalType": "uint256", "indexed": false}, {"name": "minPrice", "type": "uint256", "internalType": "uint256", "indexed": false}, {"name": "deltaPriceIncrease", "type": "uint256", "internalType": "uint256", "indexed": false}, {"name": "decreaseRate", "type": "uint256", "internalType": "uint256", "indexed": false}, {"name": "priceIncreaseDecay", "type": "uint64", "internalType": "uint64", "indexed": false}], "anonymous": false},
     {"name": "ItemTraded", "type": "event", "inputs": [{"name": "player", "type": "address", "internalType": "address", "indexed": true}, {"name": "boughtItem", "type": "address", "internalType": "address", "indexed": false}, {"name": "boughtQty", "type": "uint256", "internalType": "uint256", "indexed": false}, {"name": "soldItem", "type": "address", "internalType": "address", "indexed": false}, {"name": "soldQty", "type": "uint256", "internalType": "uint256", "indexed": false}], "anonymous": false},
     {"name": "ItemUpdated", "type": "event", "inputs": [{"name": "item", "type": "address", "internalType": "address", "indexed": true}, {"name": "currentPrice", "type": "uint256", "internalType": "uint256", "indexed": false}, {"name": "playerSellPrice", "type": "uint256", "internalType": "uint256", "indexed": false}, {"name": "minPrice", "type": "uint256", "internalType": "uint256", "indexed": false}, {"name": "deltaPriceIncrease", "type": "uint256", "internalType": "uint256", "indexed": false}, {"name": "decreaseRate", "type": "uint256", "internalType": "uint256", "indexed": false}, {"name": "priceIncreaseDecay", "type": "uint64", "internalType": "uint64", "indexed": false}, {"name": "status", "type": "uint8", "internalType": "uint8", "indexed": false}], "anonymous": false},
     {"name": "addTradeItem", "type": "function", "inputs": [{"name": "_itemAddress", "type": "address", "internalType": "address"}, {"name": "_startingPrice", "type": "uint256", "internalType": "uint256"}, {"name": "_sellPrice", "type": "uint256", "internalType": "uint256"}, {"name": "_minPrice", "type": "uint256", "internalType": "uint256"}, {"name": "_deltaPriceIncrease", "type": "uint256", "internalType": "uint256"}, {"name": "_decreaseRate", "type": "uint256", "internalType": "uint256"}, {"name": "_priceIncreaseDecay", "type": "uint64", "internalType": "uint64"}], "outputs": [], "stateMutability": "nonpayable"},
     {"name": "addressToTradeItemId", "type": "function", "inputs": [{"name": "", "type": "address", "internalType": "address"}], "outputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "stateMutability": "view"},
     {"name": "buyItem", "type": "function", "inputs": [{"name": "_itemAddress", "type": "address", "internalType": "address"}, {"name": "_quantity", "type": "uint256", "internalType": "uint256"}, {"name": "_maxPrice", "type": "uint256", "internalType": "uint256"}], "outputs": [], "stateMutability": "nonpayable"},
     {"name": "getNextPrice", "type": "function", "inputs": [{"name": "_itemAddress", "type": "address", "internalType": "address"}, {"name": "_quantity", "type": "uint256", "internalType": "uint256"}], "outputs": [{"name": "", "type": "uint256", "internalType": "uint256"}], "stateMutability": "view"},
```

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/jewel_token.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/jewel_token.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/land_auction.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/land_auction.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/land_core.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/land_core.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/master_gardener.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/master_gardener.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/meditation_circle.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/meditation_circle.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/multicall3.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/multicall3.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/pasture.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/pasture.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/pet_auction.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/pet_auction.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/pet_bridge.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/pet_bridge.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/pet_core.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/pet_core.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/pet_exchange.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/pet_exchange.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/pet_hatching.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/pet_hatching.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/power_token.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/power_token.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/power_up_manager.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/power_up_manager.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/profiles.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/profiles.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/quest_core.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/quest_core.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/raffle_master.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/raffle_master.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/raffle_ticket.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/raffle_ticket.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/stone_carver.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/stone_carver.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/stylist.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/stylist.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/token_disburse.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/token_disburse.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/uniswap_v2_factory.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/uniswap_v2_factory.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/uniswap_v2_router.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/uniswap_v2_router.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/contracts/validator_fund.py` & `dfk_contracts-0.1.7/dfk_contracts/contracts/validator_fund.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/credentials.py` & `dfk_contracts-0.1.7/dfk_contracts/credentials.py`

 * *Files identical despite different names*

### Comparing `dfk_contracts-0.1.6/dfk_contracts/solidity_types.py` & `dfk_contracts-0.1.7/dfk_contracts/solidity_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 
 from typing import Sequence, Dict, Tuple, List
 from web3.datastructures import AttributeDict
 from web3.types import TxReceipt, BlockIdentifier
-from eth_typing.evm import HexAddress
+from eth_typing.evm import ChecksumAddress
 
+HexAddress = ChecksumAddress
 # We lose some detail here; Python doesnt have signed/unsigned int differentions
-# or bytes sizes. For now, these type aliase let us use Solidity's native types 
+# or bytes sizes. For now, these type aliases let us use Solidity's native types 
 # as type hints while being a little less particular to Pythons Mypy type analyzer
-address = HexAddress
+address = ChecksumAddress
 bool = bool
 string = str
 uint8 = int
 uint16 = int
 uint32 = int
 uint64 = int
 uint128 = int
```

