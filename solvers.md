---
layout: default
---

# Solvers
## MapleCOMSPS, MapleCOMSPS_LRB, and MapleCOMSPS_CHB
* MapleCOMSPS won 1st in the SAT Competition 2016 Main track and 2nd in the Application category
* MapleCOMSPS_LRB won 1st in the SAT Competition 2016 Application category
* Based off of COMiniSatPS (a.k.a COMSPS)
* [See solver description for details](https://docs.google.com/a/gsd.uwaterloo.ca/viewer?a=v&pid=sites&srcid=Z3NkLnV3YXRlcmxvby5jYXxtYXBsZXNhdHxneDo2YWEzYjEzN2JmY2I1YzYz)
* MapleCOMSPS and MapleCOMSPS_LRB use a **LRB-VSIDS** hybrid branching heuristic; see solver description above for details
* MapleCOMSPS_CHB uses a **CHB-VSIDS** hybrid branching heuristic; see solver description above for details
* Download source code ([MapleCOMSPS_LRB](https://sites.google.com/a/gsd.uwaterloo.ca/maplesat/MapleCOMSPS_LRB.zip?attredirects=0&d=1)) ([MapleCOMSPS_CHB](https://sites.google.com/a/gsd.uwaterloo.ca/maplesat/MapleCOMSPS_CHB.zip?attredirects=0&d=1))

## MapleCOMSPS_PURE_LRB and MapleCOMSPS_PURE_CHB
* These two solvers remove VSIDS completely and replace it with either LRB or CHB; i.e., no "hybrid" branching heuristic
* Note, these two solvers were not submitted to the SAT competition
* Download source code ([MapleCOMSPS_Pure_LRB](https://sites.google.com/a/gsd.uwaterloo.ca/maplesat/MapleCOMSPS_pure_LRB.zip?attredirects=0&d=1)) ([MapleCOMSPS_Pure_CHB](https://sites.google.com/a/gsd.uwaterloo.ca/maplesat/MapleCOMSPS_pure_CHB.zip?attredirects=0&d=1))

## MapleGlucose
* Based off of Glucose 3.0
* [See solver description for details](https://docs.google.com/a/gsd.uwaterloo.ca/viewer?a=v&pid=sites&srcid=Z3NkLnV3YXRlcmxvby5jYXxtYXBsZXNhdHxneDo2OTE2OWNjODY4M2E2NmI0)
* MapleGlucose uses a **LRB-VSIDS hybrid** branching heuristic; see solver description above for details
* Download source code ([MapleGlucose](https://sites.google.com/a/gsd.uwaterloo.ca/maplesat/MapleGlucose.zip?attredirects=0&d=1))
* Call `bash starexec_build` to build

## MapleCMS
* Based off of CryptoMiniSat 4.5.3
* [See solver description for details](https://docs.google.com/a/gsd.uwaterloo.ca/viewer?a=v&pid=sites&srcid=Z3NkLnV3YXRlcmxvby5jYXxtYXBsZXNhdHxneDo2OTE2OWNjODY4M2E2NmI0)
* VSIDS is completely replaced with the **LRB** branching heuristic as described in our [SAT 2016 paper](https://docs.google.com/a/gsd.uwaterloo.ca/viewer?a=v&pid=sites&srcid=Z3NkLnV3YXRlcmxvby5jYXxtYXBsZXNhdHxneDpjODMzNWRiMzBhNDg3Yg)
* Download source code ([MapleCMS](https://sites.google.com/a/gsd.uwaterloo.ca/maplesat/MapleCMS.zip?attredirects=0&d=1))
* Call `bash starexec_build` to build

## MapleSAT
* Based off of MiniSat 2.2.0
* VSIDS is completely replaced with the **LRB** branching heuristic as described in our [SAT 2016 paper](https://docs.google.com/a/gsd.uwaterloo.ca/viewer?a=v&pid=sites&srcid=Z3NkLnV3YXRlcmxvby5jYXxtYXBsZXNhdHxneDpjODMzNWRiMzBhNDg3Yg)
* Uses LBD to perform clause deletion
* A good simple solver for understanding LRB
* [Download source code](https://sites.google.com/a/gsd.uwaterloo.ca/maplesat/MapleSAT.zip?attredirects=0&d=1)
* [Bitbucket git repository](https://bitbucket.org/JLiangWaterloo/maplesat/overview)
* Call `make` to build