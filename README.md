# CSE584Final Project

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Code](#code)

## Project Overview

This project presents an automated system designed to detect faulty science questions before they are processed by LLMs. There are 3 main research questions this project is exploring: (1)What machine learning classifier trained with labeled data performs the best to identify faulty questions? (2)Do classifiers perform differently on faulty questions in conceptual disciplines (e.g., biology) versus computational disciplines (e.g., mechanical engineering)? (3)Do faulty reason types affect classifiers’ performance?

## Dataset

Dataset of faulty science questions by different subjects: (in total 20 subjects with [5 questions + 5 similar variations] each subject)

https://docs.google.com/spreadsheets/d/1pxm7_-M4s6ygUYinye24H0nI1a0N3je831xULYvl2jE/edit?usp=sharing

My experimental columns: (personally added last two columns)

| Discipline | Question | Reason you think it is faulty | Which top LLM you tried | Response by the top LLM | Original correct question | Faulty Reason Type |

The original correct science questions come from: (StemQ, ScienceQA) *I edited the questions to make them faulty and try to fool LLM.

https://github.com/idrori/stemQ

https://github.com/lupantech/ScienceQA

See data100.csv for 100 rows of data, which merged all subjects and shuffled.

See data200.csv for 200 rows of augmented data, which merged all subjects and shuffled.

## Code

Runnable code and experiment results on Colab:

https://colab.research.google.com/drive/1LYpkCz61HEwWOn3uw3yC0yvPBAMnCh7u?usp=sharing

