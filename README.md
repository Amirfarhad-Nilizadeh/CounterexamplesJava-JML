# CounterexamplesJava-JML

This repository has the results of dynamic APR tools of a submitted paper.

For this study, we used all 256 not verified repaired programs from the buggy [Java+JML dataset](https://github.com/Amirfarhad-Nilizadeh/BuggyJavaJML):
1)  OpenJML's ESC generates counterexamples for all programs.
2)  Using runtime assertion checking of OpenJML, we classified all repaired programs to overfitted and formal method's false negatives.
3)  Counterexamples are added to the initial test suite of each program, and dynamic APR tools are run on all not verified programs.

Our results show that dynamic APR tools generating about 83.6% fewer overfitted patches which 27.4% were correct patches, and in other cases correct patch was not in their candidate patches. However, in about 16.4%, these APR tools again generated overfitted patches, while they did not generate the same overfitted patch. 

You can see the newly overfitted patches in this repository when counterexamples were added to the test suite. [In this link](https://anonymous.4open.science/r/BuggyJavaJML-8EE2/ReadMe.md), you can find counterexamples for all not verified programs. 
