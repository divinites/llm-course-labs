# LLM course labs

Exercises for the Large Language Models course. You need a Google account and a browser. There is no code to write and nothing to install.

| Lecture | Lab | Open it |
|---|---|---|
| 3 | Distil a spam filter: copy a 125-million-dial model into a 16,000-dial one, and see what gets lost | [Open in Colab](https://colab.research.google.com/github/divinites/llm-course-labs/blob/main/distil_a_spam_filter.ipynb) |

A dial is a parameter: a number the model adjusts during training.

## What is in here

- `distil_a_spam_filter.ipynb`: the notebook. Press **Runtime > Run all**, then change the numbers at the top.
- `teacher_scores.json`: the teacher's raw scores on all 5,574 messages, in the order of the dataset. We computed them in advance, so that you do not need a GPU. The notebook can also compute them itself: set `RUN_TEACHER_YOURSELF = True`.

## Data and models

- Messages: [SMS Spam Collection](https://archive.ics.uci.edu/dataset/228/sms+spam+collection), Almeida, Gómez Hidalgo and Yamakami (2011), CC BY 4.0. They are real messages, and some spam is rude. The notebook downloads them when it runs.
- Teacher: [`mshenoda/roberta-spam`](https://huggingface.co/mshenoda/roberta-spam), downloaded when the notebook runs.
