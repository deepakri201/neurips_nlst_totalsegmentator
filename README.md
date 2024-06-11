# **Rule-based outlier detection of AI-generated anatomy segmentations**

**Deepa Krishnaswamy, Vamsi Krishna Thiriveedhi, Cosmin Ciausu, David Clunie,Steve Pieper, Ron Kikinis, Andrey Fedorov**

*Submitted to NeurIPS Datasets and Benchmarks Track 2024*

---

This repository and notebook provides the code that is needed to reproduce the figures in the paper submitted to NeurIPS Datasets and Benchmarks track. 

In the Parameterization and setup section, users will download `parquet` files to have access to various qualitative and quantitative measurements. These will then be queried using `duckdb` for the two studies: 
1. Comparison of left vs right ribs in terms of volume: Here we compute the normalized difference in volume between the left and right ribs. We do this for each sequential addition of the heuristics, starting with original data, segmentation completeness check, connected components check, volume >5 mL check, and laterality check. We then perform statistics to see if there is an effect of each additional heuristic. 
2. Population study of the vertebrae. In this section, we obtain the volume of each vertebra and form two groups based on males vs females. We apply the same heuristics as the above. We then compare these volumes to those from a population study and obesrve if the trends are similar. 

---

Deepa Krishnaswamy and Vamsi Krishna Thiriveedhi

Brigham and Women's Hospital 

June 2024
