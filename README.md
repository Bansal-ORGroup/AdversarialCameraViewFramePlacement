# AdversarialCameraViewFramePlacement

# Seonghun Park and Manish Bansal
This repository is a companion repository for the paper titled "Algorithms for Cameras View-Frame Placement Problems in the Presence of an Adversary and Distributional Ambiguity." (Link to paper: [Click](https://optimization-online.org/wp-content/uploads/2023/04/ParkBansal-ArXiv-4-10-2023.pdf))

## Abstract:

In this paper, we introduce cameras view-frame placement problem (denoted by CFP) in the presence of an adversary whose objective is to minimize the maximum coverage by $p$ cameras in response to input provided by $n$ autonomous agents in a remote location. We allow uncertainty in the success of attacks, incomplete information of the probability distribution associated with the uncertain data, and varying levels of risk-appetite of the adversary. We present an exact cutting planes based algorithm to solve this problem along with conditions under which it is finitely convergent. Since this approach solves deterministic CFP in each iteration, we also present improved exact method for CFP with $p=1$, approximation algorithm and heuristics for Multi-CFP with $p\geq 2$, and Multi-CFP with fixed tilt of the cameras. To evaluate the effectiveness and performance of the proposed approaches, we conduct computational experiments using randomly generated instances and simulation experiments where these approaches are utilized to find a hidden object in a remote location.

## Data:

Within the "instance" directory, there are subfolders named according to the particular problem we address in our paper. The "Demand" subfolder contains the generated request used in our tests, while the "realization" subfolder stores produced realzation vectors.Each instance is stored in a pickle file, with its name containing two descriptive numbers. The first number indicates the count of requests, while the second represents the replication number. 

## Loading Data from Pickle File

To load the `demand_10_0.pickle` dataset into your workspace using Python, follow the example code provided below:

```
import pandas as pd
import pickle

data = pd.read_pickle('./demand_10_0.pickle')
```
For a detailed procedure on instance generation, refer to our paper. (Link to paper: [Click](https://optimization-online.org/wp-content/uploads/2023/04/ParkBansal-ArXiv-4-10-2023.pdf))
