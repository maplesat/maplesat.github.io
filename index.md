---
layout: default
---

# MapleSAT: A Machine Learning based SAT Solver
The Maple series of SAT solvers is a family of  conflict-driven clause-learning SAT solvers outfitted with machine learning-based heuristics. Currently MapleSAT supports machine learning based branching and restarts policies. In the future, we plan to add a machine learning based clause learning policy.

A key innovation in the MapleSAT series of SAT solvers is the use of the **learning rate branching heuristic (LRB)**, a departure from the VSIDS branching heuristic that has been the status quo for the past decade of SAT solving. (Note that the experiments in our SAT 2016 paper describing LRB use only pure branching heuristics. That is, the VSIDS experiment uses only VSIDS and the LRB experiments uses only LRB. The hybrid LRB-VSIDS branching heuristic in MapleCOMSPS and MapleGlucose is only for the SAT competition and not part of the SAT 2016 paper.)
