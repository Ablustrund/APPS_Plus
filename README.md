# APPS_Plus
This is the repository for [StepCoder: Improving Code Generation with Reinforcement Learning from Compiler Feedback](https://arxiv.org/pdf/2402.01391.pdf).
## Summary

👉 08/31/2024. We clean the function name of the canonical solution in each programming problem. The final version of our APPS+ dataset is available at here: https://drive.usercontent.google.com/download?id=1dTRJHXhMcPz4CPt73f2vju5KdLmqcP4F&export=download&authuser=0

👉 The new version of our APPS+ dataset is available at here: https://drive.google.com/file/d/1wfrDRcvAn38qj5dDmQZwaoLIAmT4q7KQ/view?usp=sharing


Based on APPS, we released the first version of the apps+ data, and we will further manually refine it, which is expected to increase the average number of unit tests to 15! 


👉**APPS+ is refined from [APPS](https://github.com/hendrycks/apps) and contains programming problems from open-access sites, including Codewars, AtCoder, Kattis, and Codeforces.**

## Refinement
To refine the APPS dataset, we excluded instances lacking input, output, or canonical solutions. Then, we standardized the formats of input and output to facilitate the execution and comparison of unit tests. We conducted unit tests and manual analysis for each instance, eliminating those with incomplete or irrelevant code, syntax errors, API misuse, or missing library dependencies. For discrepancies in output, we manually reviewed the problem description, correcting the expected output or eliminating the instance.

Finally, we construct the APPS+ dataset, containing 7,413 instances (introductory: 2889, interview: 3592, competition: 572). Each instance includes a programming problem description, a canonical solution, a function name, unit tests (i.e., inputs and outputs), and starter code (i.e., the beginning part of the canonical solution). 

## Acknowledgement
```
@article{hendrycksapps2021,
  title={Measuring Coding Challenge Competence With APPS},
  author={Dan Hendrycks and Steven Basart and Saurav Kadavath and Mantas Mazeika and Akul Arora and Ethan Guo and Collin Burns and Samir Puranik and Horace He and Dawn Song and Jacob Steinhardt},
  journal={NeurIPS},
  year={2021}
}
```


## Citation
If you find this useful in your research, please consider citing
```
@article{dou2024stepcoder,
  title={StepCoder: Improve Code Generation with Reinforcement Learning from Compiler Feedback},
  author={Dou, Shihan and Liu, Yan and Jia, Haoxiang and Xiong, Limao and Zhou, Enyu and Shan, Junjie and Huang, Caishuang and Shen, Wei and Fan, Xiaoran and Xi, Zhiheng and others},
  journal={arXiv preprint arXiv:2402.01391},
  year={2024}
}
```

