# CAN-QA: A-Question-Answering-Benchmark-for-Reasoning-over-In-Vehicle-CAN-Traffic

This repository contains the source code for the framework introduced in https://arxiv.org/abs/2604.24935.

There are 2 main folders in this repo: 
1. Dataset: This folder contains the preprocessing file that can be used on any dataset. All the processed data will also go in this folder
2. QA: This folder contains all the code that will create the Question-Answer pairs from your dataset. It contains 2 more folders which represent the True-False question code or the Multiple Choice Answer code. 

For the folders inside the QA folder, both folders contain the same files which are tuned to create either True/False or MCQ Questions. Inside those folders we specifically have: 
1. Create_... - This file creates the respective questions based on the data you provided in the Dataset folder.
2. Answer_... - This file uses a model of your choice to answer the questions generated from the Create_... file.
3. Evaluations_... - This file takes the answers generated from the Answer_... file and compares it with the ground truth answers. Then, it uses all that data to create a comprehensive report of how well the chosen model fared.

# Citation

This code can be used for research purposes as long as you have an appropriate citation: 

~~~
@misc{chen2026can,
      title={CAN-QA: A Question-Answering Benchmark for Reasoning over In-Vehicle CAN Traffic}, 
      author={Jing Chen and Abhijay Deevi and Onat Gungor and Tajana Rosing},
      year={2026},
      eprint={2604.24935},
      archivePrefix={arXiv},
      primaryClass={cs.CR},
      url={https://arxiv.org/abs/2604.24935}, 
}
~~~
