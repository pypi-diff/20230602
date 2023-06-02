# Comparing `tmp/pref_voting-0.4.7.tar.gz` & `tmp/pref_voting-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-0.4.7.tar", max compression
+gzip compressed data, was "pref_voting-0.4.8.tar", max compression
```

## Comparing `pref_voting-0.4.7.tar` & `pref_voting-0.4.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.4.7/LICENSE
--rw-r--r--   0        0        0     3445 2023-06-01 15:01:07.264675 pref_voting-0.4.7/README.md
--rw-r--r--   0        0        0       22 2023-06-02 02:53:48.066221 pref_voting-0.4.7/pref_voting/__init__.py
--rw-r--r--   0        0        0     9632 2023-05-24 13:13:44.583927 pref_voting-0.4.7/pref_voting/analysis.py
--rw-r--r--   0        0        0     1226 2023-05-24 13:13:43.582814 pref_voting-0.4.7/pref_voting/axiom.py
--rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.4.7/pref_voting/axiom_helpers.py
--rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-0.4.7/pref_voting/axioms.py
--rw-r--r--   0        0        0    23065 2023-05-10 11:22:02.837497 pref_voting-0.4.7/pref_voting/c1_methods.py
--rw-r--r--   0        0        0     8551 2023-05-30 17:01:09.832556 pref_voting-0.4.7/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    11517 2023-05-10 11:58:43.699679 pref_voting-0.4.7/pref_voting/dominance_axioms.py
--rw-r--r--   0        0        0    20643 2023-05-10 11:16:22.353419 pref_voting-0.4.7/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0     4347 2023-06-01 14:59:17.885777 pref_voting-0.4.7/pref_voting/generate_spatial_profiles.py
--rw-r--r--   0        0        0     4874 2023-06-01 02:28:51.128709 pref_voting-0.4.7/pref_voting/generate_utility_profiles.py
--rw-r--r--   0        0        0    10486 2023-05-24 13:13:45.272860 pref_voting-0.4.7/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.4.7/pref_voting/helper.py
--rw-r--r--   0        0        0    77209 2023-06-01 16:34:57.903960 pref_voting-0.4.7/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.4.7/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    59218 2023-05-26 17:44:51.542166 pref_voting-0.4.7/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    25681 2023-05-10 11:20:32.560828 pref_voting-0.4.7/pref_voting/other_methods.py
--rw-r--r--   0        0        0    28614 2023-05-30 20:06:31.706933 pref_voting-0.4.7/pref_voting/profiles.py
--rw-r--r--   0        0        0    25273 2023-05-26 17:38:33.040884 pref_voting-0.4.7/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    12468 2023-05-26 10:23:18.532269 pref_voting-0.4.7/pref_voting/rankings.py
--rw-r--r--   0        0        0    11066 2023-05-26 12:19:11.420399 pref_voting-0.4.7/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     6840 2023-06-01 14:59:19.931166 pref_voting-0.4.7/pref_voting/spatial_profiles.py
--rw-r--r--   0        0        0     3066 2023-05-31 23:53:43.134760 pref_voting-0.4.7/pref_voting/utility_functions.py
--rw-r--r--   0        0        0     6661 2023-05-26 14:18:34.309764 pref_voting-0.4.7/pref_voting/utility_methods.py
--rw-r--r--   0        0        0    15702 2023-06-02 02:53:42.477653 pref_voting-0.4.7/pref_voting/utility_profiles.py
--rw-r--r--   0        0        0     8393 2023-05-26 10:50:34.876976 pref_voting-0.4.7/pref_voting/variable_voter_axioms.py
--rw-r--r--   0        0        0     5395 2023-05-26 10:54:32.445716 pref_voting-0.4.7/pref_voting/voting_method.py
--rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.4.7/pref_voting/voting_methods.py
--rw-r--r--   0        0        0    53001 2023-05-26 17:56:28.071379 pref_voting-0.4.7/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      689 2023-06-02 02:53:48.065485 pref_voting-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     4400 1970-01-01 00:00:00.000000 pref_voting-0.4.7/setup.py
--rw-r--r--   0        0        0     4513 1970-01-01 00:00:00.000000 pref_voting-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.4.8/LICENSE
+-rw-r--r--   0        0        0     3528 2023-06-02 10:11:51.114635 pref_voting-0.4.8/README.md
+-rw-r--r--   0        0        0       22 2023-06-02 10:11:56.283855 pref_voting-0.4.8/pref_voting/__init__.py
+-rw-r--r--   0        0        0     9632 2023-05-24 13:13:44.583927 pref_voting-0.4.8/pref_voting/analysis.py
+-rw-r--r--   0        0        0     1226 2023-05-24 13:13:43.582814 pref_voting-0.4.8/pref_voting/axiom.py
+-rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.4.8/pref_voting/axiom_helpers.py
+-rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-0.4.8/pref_voting/axioms.py
+-rw-r--r--   0        0        0    23065 2023-05-10 11:22:02.837497 pref_voting-0.4.8/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0     8551 2023-05-30 17:01:09.832556 pref_voting-0.4.8/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    11517 2023-05-10 11:58:43.699679 pref_voting-0.4.8/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    20643 2023-05-10 11:16:22.353419 pref_voting-0.4.8/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0     4347 2023-06-01 14:59:17.885777 pref_voting-0.4.8/pref_voting/generate_spatial_profiles.py
+-rw-r--r--   0        0        0     4874 2023-06-01 02:28:51.128709 pref_voting-0.4.8/pref_voting/generate_utility_profiles.py
+-rw-r--r--   0        0        0    10486 2023-05-24 13:13:45.272860 pref_voting-0.4.8/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.4.8/pref_voting/helper.py
+-rw-r--r--   0        0        0    80807 2023-06-02 10:13:04.013698 pref_voting-0.4.8/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.4.8/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    59218 2023-05-26 17:44:51.542166 pref_voting-0.4.8/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    25681 2023-05-10 11:20:32.560828 pref_voting-0.4.8/pref_voting/other_methods.py
+-rw-r--r--   0        0        0    28614 2023-05-30 20:06:31.706933 pref_voting-0.4.8/pref_voting/profiles.py
+-rw-r--r--   0        0        0    25273 2023-05-26 17:38:33.040884 pref_voting-0.4.8/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    12468 2023-05-26 10:23:18.532269 pref_voting-0.4.8/pref_voting/rankings.py
+-rw-r--r--   0        0        0    11066 2023-05-26 12:19:11.420399 pref_voting-0.4.8/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     6840 2023-06-01 14:59:19.931166 pref_voting-0.4.8/pref_voting/spatial_profiles.py
+-rw-r--r--   0        0        0     3066 2023-05-31 23:53:43.134760 pref_voting-0.4.8/pref_voting/utility_functions.py
+-rw-r--r--   0        0        0     6661 2023-05-26 14:18:34.309764 pref_voting-0.4.8/pref_voting/utility_methods.py
+-rw-r--r--   0        0        0    15702 2023-06-02 02:53:42.477653 pref_voting-0.4.8/pref_voting/utility_profiles.py
+-rw-r--r--   0        0        0     8393 2023-05-26 10:50:34.876976 pref_voting-0.4.8/pref_voting/variable_voter_axioms.py
+-rw-r--r--   0        0        0     5395 2023-05-26 10:54:32.445716 pref_voting-0.4.8/pref_voting/voting_method.py
+-rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.4.8/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0    53001 2023-05-26 17:56:28.071379 pref_voting-0.4.8/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      689 2023-06-02 10:11:56.282805 pref_voting-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     4485 1970-01-01 00:00:00.000000 pref_voting-0.4.8/setup.py
+-rw-r--r--   0        0        0     4596 1970-01-01 00:00:00.000000 pref_voting-0.4.8/PKG-INFO
```

### Comparing `pref_voting-0.4.7/LICENSE` & `pref_voting-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/README.md` & `pref_voting-0.4.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,16 @@
 - v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
 - v0.2.8 (2023-5-16): Add description function to Majority Graphs.
 - v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.
 - v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.
 - v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies
 - v0.3.3 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.
 - v0.3.4 (2023-5-30): Add write and from_string methods to a UtilityProfile.
-- v0.4.3 (2023-5-31): Add SpatialProfile class and utility functions for generating utility profiles from spatial profiles; add functions to generate a SpatialProfile.
+- v0.4.7 (2023-5-31): Add SpatialProfile class and utility functions for generating utility profiles from spatial profiles; add functions to generate a SpatialProfile.
+- v0.4.8 (2023-5-31): Add bottom two IRV and Tideman's alternative voting methods.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

### Comparing `pref_voting-0.4.7/pref_voting/analysis.py` & `pref_voting-0.4.8/pref_voting/analysis.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/axiom.py` & `pref_voting-0.4.8/pref_voting/axiom.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/c1_methods.py` & `pref_voting-0.4.8/pref_voting/c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/combined_methods.py` & `pref_voting-0.4.8/pref_voting/combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/dominance_axioms.py` & `pref_voting-0.4.8/pref_voting/dominance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/generate_profiles.py` & `pref_voting-0.4.8/pref_voting/generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/generate_spatial_profiles.py` & `pref_voting-0.4.8/pref_voting/generate_spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/generate_utility_profiles.py` & `pref_voting-0.4.8/pref_voting/generate_utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-0.4.8/pref_voting/generate_weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/helper.py` & `pref_voting-0.4.8/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/iterative_methods.py` & `pref_voting-0.4.8/pref_voting/iterative_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
     File: iterative_methods.py
     Author: Eric Pacuit (epacuit@umd.edu)
     Date: January 6, 2022
     Update: July 23, 2022
     
     Implementations of iterative voting methods.
 '''
-
 from pref_voting.voting_method import  *
 from pref_voting.voting_method import _num_rank_last, _num_rank_first
 from pref_voting.profiles import  _borda_score, _find_updated_profile
 from pref_voting.margin_based_methods import split_cycle, minimax_scores
+from pref_voting.c1_methods import top_cycle, gocha
 
 import copy
 from itertools import permutations, product
 import numpy as np
 
 @vm(name = "Instant Runoff")
 def instant_runoff(profile, curr_cands = None):
@@ -403,14 +403,54 @@
     reduced_prof.remove_empty_rankings()
         
     pl_scores = reduced_prof.plurality_scores()
     
     max_pl_score = max(pl_scores.values())
     
     return sorted([c for c in pl_scores.keys() if pl_scores[c] == max_pl_score])
+
+@vm(name="Bottom-Two-Runoff Instant Runoff")
+def bottom_two_runoff_instant_runoff(profile, curr_cands = None):
+    """Find the two candidates with the lowest two plurality scores, remove the one who loses head-to-head to the other, and repeat until a single candidate remains. Parallel-universe tiebreaking is used to break ties for lowest or second lowest plurality scores. 
+
+    .. note:: 
+        BTR-IRV is a Condorcet consistent voting method, i.e., if a Condorcet winner exists, then BTR-IRV will elect the Condorcet winner. 
+
+    Args:
+        profile (Profile): An anonymous profile of linear orders on a set of candidates
+        curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
+
+    Returns: 
+        A sorted list of candidates
+    """
+    candidates = profile.candidates if curr_cands is None else curr_cands 
+
+    if len(candidates) == 1:
+        return candidates
+
+    cands_with_lowest_plurality_score = [cand for cand, value in profile.plurality_scores(candidates).items() if value == min(profile.plurality_scores(candidates).values())]
+
+    if len(cands_with_lowest_plurality_score) > 1:
+        cands_with_second_lowest_plurality_score = cands_with_lowest_plurality_score
+    else:
+        cands_with_second_lowest_plurality_score = [cand for cand, value in profile.plurality_scores(candidates).items() if value == sorted(profile.plurality_scores(candidates).values())[1]]
+    
+    winners = []
+
+    for c1 in cands_with_lowest_plurality_score:
+        for c2 in cands_with_second_lowest_plurality_score:
+            if c1 != c2:
+                if profile.margin(c1,c2) <= 0:
+                    additional_winners = bottom_two_runoff_instant_runoff(profile, curr_cands = [c for c in candidates if not c == c1])
+                else:
+                    additional_winners = bottom_two_runoff_instant_runoff(profile, curr_cands = [c for c in candidates if not c == c2])
+                
+                winners = winners + additional_winners
+    
+    return sorted(set(winners))
     
 @vm(name = "PluralityWRunoff")
 def plurality_with_runoff(profile, curr_cands = None):
     """If there is a majority winner then that candidate is the plurality with runoff winner. If there is no majority winner, then hold a runoff with  the top two candidates: either two (or more candidates) with the most first place votes or the candidate with the most first place votes and the candidate with the 2nd highest first place votes are ranked first by the fewest number of voters.   A candidate is a Plurality with Runoff winner in the profile restricted to ``curr_cands`` if it is a winner in a runoff between two pairs of first- or second- ranked candidates. If the candidates are all tied for the most first place votes, then all candidates are winners.
         
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
@@ -783,15 +823,15 @@
     return sorted(winners), elims_list
 
 @vm(name = "Baldwin")
 def baldwin(profile, curr_cands = None):
     """Iteratively remove all candidates with the lowest Borda score until a single candidate remains.  If, at any stage, all  candidates have the same Borda score,  then all (remaining) candidates are winners.
 
     .. note:: 
-        Baldwin is a Condorcet consistent voting method means that if a Condorcet winner exists, then Baldwin will elect the Condorcet winner. 
+        Baldwin is a Condorcet consistent voting method, i.e., if a Condorcet winner exists, then Baldwin will elect the Condorcet winner. 
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
@@ -1081,15 +1121,15 @@
 
 @vm(name = "Strict Nanson")
 def strict_nanson(profile, curr_cands = None):
     """Iteratively remove all candidates with the  Borda score strictly below the average Borda score until one candidate remains.  If, at any stage, all  candidates have the same Borda score, then all (remaining) candidates are winners.
 
     .. note:: 
         
-        Strict Nanson is a Condorcet consistent voting method means that if a Condorcet winner exists, then Strict Nanson will elect the Condorcet winner. 
+        Strict Nanson is a Condorcet consistent voting method, i.e., if a Condorcet winner exists, then Strict Nanson will elect the Condorcet winner. 
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
@@ -1225,15 +1265,15 @@
 
 @vm(name = "Weak Nanson")
 def weak_nanson(profile, curr_cands = None):
     """Iteratively remove all candidates with Borda score less than or equal the average Borda score until one candidate remains.  If, at any stage, all  candidates have the same Borda score, then all (remaining) candidates are winners.
 
     .. note:: 
 
-        Weak Nanson is a Condorcet consistent voting method means that if a Condorcet winner exists, then Weak Nanson will elect the Condorcet winner. 
+        Weak Nanson is a Condorcet consistent voting method, i.e.,  if a Condorcet winner exists, then Weak Nanson will elect the Condorcet winner. 
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
@@ -1696,41 +1736,78 @@
             candidates = vm_ws
             vm_ws = vm(edata, curr_cands=candidates)
 
         return vm_ws
 
     return VotingMethod(_vm, name=f"Iterated {vm.name}")
 
+def tideman_alternative(vm):
+    """Given a voting method vm, returns a voting method that restricts the profile to the set of vm winners, then eliminates the candidate with the fewest first-place votes, and then repeats until there is only one vm winner. Parallel-universe tiebreaking is used when there are multiple candidates with the fewest first-place votes.
+
+    Args:
+        vm (VotingMethod): A voting method.
+
+    Returns:
+        The Tideman Alternative version of vm.
+
+    """
+    
+    def _ta(profile, curr_cands = None):
+
+        candidates = profile.candidates if curr_cands is None else curr_cands 
+    
+        vm_ws = vm(profile, curr_cands = candidates)
+
+        if len(vm_ws) == 1:
+            return vm_ws
+    
+        else: 
+            cands_to_remove = [cand for cand, value in profile.plurality_scores(vm_ws).items() if value == min(profile.plurality_scores(vm_ws).values())]
+        
+            winners = []
+            for cand_to_remove in cands_to_remove:
+                additional_winners = _ta(profile, curr_cands = [c for c in candidates if not c == cand_to_remove])
+                winners = winners + additional_winners
+
+        return sorted(set(winners))
+
+    return VotingMethod(_ta, name=f"Tideman Alternative {vm.name}")
+
+tideman_alternative_smith = tideman_alternative(top_cycle)
+tideman_alternative_schwartz = tideman_alternative(gocha)
+
     
 iterated_vms = [
     instant_runoff,
     instant_runoff_tb,
     instant_runoff_put,
     hare,
     ranked_choice,
+    bottom_two_runoff_instant_runoff,
+    benham,
+    benham_put,
+    benham_tb
     plurality_with_runoff,
     coombs,
     coombs_tb,
     coombs_put,
-    strict_nanson,
-    weak_nanson,
     baldwin,
     baldwin_tb,
     baldwin_put,
+    strict_nanson,
+    weak_nanson,
     iterated_removal_cl,
     iterated_removal_worst_losers,
     iterated_split_cycle,
-    benham,
-    benham_put,
-    benham_tb
+    tideman_alternative_smith,
+    tideman_alternative_schwartz
 ]
 
 iterated_vms_with_explanation = [
     instant_runoff_with_explanation,
     coombs_with_explanation,
     plurality_with_runoff_with_explanation,
     baldwin_with_explanation,
     strict_nanson_with_explanation,
     weak_nanson_with_explanation,
     iterated_removal_cl_with_explanation,
-]
-
+]
```

### Comparing `pref_voting-0.4.7/pref_voting/maj_graph_ex1.png` & `pref_voting-0.4.8/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/margin_based_methods.py` & `pref_voting-0.4.8/pref_voting/margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/other_methods.py` & `pref_voting-0.4.8/pref_voting/other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/profiles.py` & `pref_voting-0.4.8/pref_voting/profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/profiles_with_ties.py` & `pref_voting-0.4.8/pref_voting/profiles_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/rankings.py` & `pref_voting-0.4.8/pref_voting/rankings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/scoring_methods.py` & `pref_voting-0.4.8/pref_voting/scoring_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/spatial_profiles.py` & `pref_voting-0.4.8/pref_voting/spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/utility_functions.py` & `pref_voting-0.4.8/pref_voting/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/utility_methods.py` & `pref_voting-0.4.8/pref_voting/utility_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/utility_profiles.py` & `pref_voting-0.4.8/pref_voting/utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/variable_voter_axioms.py` & `pref_voting-0.4.8/pref_voting/variable_voter_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/voting_method.py` & `pref_voting-0.4.8/pref_voting/voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pref_voting/weighted_majority_graphs.py` & `pref_voting-0.4.8/pref_voting/weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.4.7/pyproject.toml` & `pref_voting-0.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "0.4.7"
+version = "0.4.8"
 description = "pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
```

### Comparing `pref_voting-0.4.7/setup.py` & `pref_voting-0.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'networkx>=3.0,<4.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '0.4.7',
+    'version': '0.4.8',
     'description': 'pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of voting methods.',
-    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.\n- v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.\n- v0.2.8 (2023-5-16): Add description function to Majority Graphs.\n- v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.\n- v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.\n- v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies\n- v0.3.3 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.\n- v0.3.4 (2023-5-30): Add write and from_string methods to a UtilityProfile.\n- v0.4.3 (2023-5-31): Add SpatialProfile class and utility functions for generating utility profiles from spatial profiles; add functions to generate a SpatialProfile.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
+    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.\n- v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.\n- v0.2.8 (2023-5-16): Add description function to Majority Graphs.\n- v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.\n- v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.\n- v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies\n- v0.3.3 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.\n- v0.3.4 (2023-5-30): Add write and from_string methods to a UtilityProfile.\n- v0.4.7 (2023-5-31): Add SpatialProfile class and utility functions for generating utility profiles from spatial profiles; add functions to generate a SpatialProfile.\n- v0.4.8 (2023-5-31): Add bottom two IRV and Tideman\'s alternative voting methods.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pref_voting-0.4.7/PKG-INFO` & `pref_voting-0.4.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 0.4.7
+Version: 0.4.8
 Summary: pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -86,15 +86,16 @@
 - v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
 - v0.2.8 (2023-5-16): Add description function to Majority Graphs.
 - v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.
 - v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.
 - v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies
 - v0.3.3 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.
 - v0.3.4 (2023-5-30): Add write and from_string methods to a UtilityProfile.
-- v0.4.3 (2023-5-31): Add SpatialProfile class and utility functions for generating utility profiles from spatial profiles; add functions to generate a SpatialProfile.
+- v0.4.7 (2023-5-31): Add SpatialProfile class and utility functions for generating utility profiles from spatial profiles; add functions to generate a SpatialProfile.
+- v0.4.8 (2023-5-31): Add bottom two IRV and Tideman's alternative voting methods.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

