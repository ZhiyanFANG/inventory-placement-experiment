# inventory-placement-experiment
Code of Chapter 6: Numerical Experiments in the Master Thesis of Zhiyan FANG, Institute of Operations Research and Analytics, National University of Singapore.

These experiments are conducted to compare the performance of our proposed Guaranteed-Delay Replenishment Model (GDRM) and one typical traditional model (Graves and Willems, 2003). The bulldozer supply chain for experiments is shown as below.

![supply-chain](https://github.com/ZhiyanFANG/inventory-placement-experiment/blob/main/supply-chain.png)

Each folder represents a different assumption of demand arrival:

| Folder | Assumption |
| ------------- | ------------- |
| `Exp-Bio1,2` | Dense Demand Arrival: demand inter-arrival times take 1 or 2, and obey Bernoulli distribution |
| `Exp-Bio29,30` | Sparse Demand Arrival: demand inter-arrival times take 29 or 30, and obey Bernoulli distribution |
| `Exp-GeLong` | Dense Demand Arrival: demand inter-arrival times take 1, 2 or 3, and obey some general distribution |
| `Exp-GeShort` | Sparse Demand Arrival: demand inter-arrival times take 10, 20 or 30, and obey some general distribution |

and in each folder, there are following files.

| File | Explanation |
| ------------- | ------------- |
| `New-Model.ipynb` | Optimize GDRM and conduct simulation under Poisson/general distributed demand assumption |
| `Traditional-Model.ipynb` | Optimize Graves and Willems' model and conduct simulation under Poisson/general distributed demand assumption |
| `Traditional-k-Selection.ipynb` | Collect output data and draw boxplots |
| `FSSFile.txt` | Store the part 1 output matrix of our proposed algorithm |
| `Trad-Solution.txt` | Store the solution of Graves and Willems' model |
| `New-General-Simulation | Store the simulation result under general distributed demand assumption of our GDRM |
| `New-Poisson-Simulation | Store the simulation result under Poisson distributed demand assumption of our GDRM |
| `Trad-General-Simulation | Store the simulation result under general distributed demand assumption of Graves and Willems' model |
| `Trad-Poisson-Simulation | Store the simulation result under Poisson distributed demand assumption of Graves and Willems' model |

In the above files, we conduct both **model optimization** and **simulation** for both types of inventory placement models.

Please refer to the thesis for detailed information.
