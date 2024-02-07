# APPS_Plus
This is the repository for [StepCoder: Improve Code Generation with Reinforcement Learning from Compiler Feedback](https://arxiv.org/pdf/2402.01391.pdf).
## Summary
Based on APPS, we released the first version of the apps+ data, and we will further manually refine it, which is expected to increase the average number of unit tests to 15! **Noted that APPS+ contains programming problems from open-access sites, including Codewars, AtCoder, Kattis, and Codeforces.**
## Refinement
To refine the APPS dataset, we excluded instances lacking input, output, or canonical solutions. Then, we standardized the formats of input and output to facilitate the execution and comparison of unit tests. We conducted unit tests and manual analysis for each instance, eliminating those with incomplete or irrelevant code, syntax errors, API misuse, or missing library dependencies. For discrepancies in output, we manually reviewed the problem description, correcting the expected output or eliminating the instance.

Finally, we construct the APPS+ dataset, containing 7,413 instances (introductory: 2889, interview: 3592, competition: 572). Each instance includes a programming problem description, a canonical solution, a function name, unit tests (i.e., inputs and outputs), and starter code (i.e., the beginning part of the canonical solution). 
## Citation
```
@misc{dou2024stepcoder,
      title={StepCoder: Improve Code Generation with Reinforcement Learning from Compiler Feedback}, 
      author={Shihan Dou and Yan Liu and Haoxiang Jia and Limao Xiong and Enyu Zhou and Wei Shen and Junjie Shan and Caishuang Huang and Xiao Wang and Xiaoran Fan and Zhiheng Xi and Yuhao Zhou and Tao Ji and Rui Zheng and Qi Zhang and Xuanjing Huang and Tao Gui},
      year={2024},
      eprint={2402.01391},
      archivePrefix={arXiv},
      primaryClass={cs.SE}
}
```

