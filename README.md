# Problem Solving with Python — Chapter 17: Build Prediction Models

This repository contains the chapter and active-learning exercise code associated with this chapter in the book *Problem Solving with Python: Using Computational Thinking in Everyday Life* by Michael D. Smith (2026), which is available from [MIT Press](https://mitpress.mit.edu/9780262383677/problem-solving-with-python/) and [Amazon](https://www.amazon.com/Problem-Solving-Python-Computational-Thinking/dp/0262552841/).

## Getting started

You will need:

- an integrated development environment (IDE)
- Python 3.10 or newer
- `pip` (usually included with Python)

If you need help getting started with an IDE, please read [my short introduction to "Understanding and Selecting an IDE"](https://ctps.io/select_ide.html).

The book's chapter describes how you can download the Ames Iowa Housing data from Kaggle, which you need as input for the scripts.

## Cloning this repository

If you're using GitHub Codespaces, click the green "Code" button on this repo's page, select the tab "Codespaces," and click the "Create codespace on main."

Otherwise, in your IDE's terminal window, type the following commands:

```bash
git clone https://github.com/pswp-book/chap17.git
cd chap17
```

## (Optional) Create and activate a virtual environment

```bash
python -m venv .venv
# Windows
.\.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate
```

## Install dependencies

```bash
pip install -r requirements.txt
```

If there is no file `requirements.txt`, the code in this repository uses only the Python standard library.

## Reporting issues

If you find a problem in this chapter’s code (typo, bug, or mismatch with the book):

1.  Check the issues for this repo to see if it’s already reported.

2.  Open a new issue and include:
    *   The chapter number and section title (e.g., “Chapter 5, The game loop”)
    *   The filename, line number(s), and a short description of the problem.
    *   If something's wrong with the code's execution, please describe how you ran the program and the exeuction result.

## Short description of the repo's files

`head.py`: Prints the first 5 rows of the specified CSV file.
This script assumes that the input file has a header row.

`get_header.py`: Jim Waldo's utility that grabs the header
from a CSV file and writes each column label on a separate
indexed line.

`avg_pbbr.py`: Computes the average home price by count
of bedrooms. Custom-made for the Ames-Iowa-Housing data set.

`desc.py`: Reads tabular CSV data into a Panda DataFrame
and uses `pandas.DataFrame.describe` to print some descriptive
statistics by column.

`ames.ipynb`: A Python notebook containing the code used
in Chapter 17 to investigate the Ames-Iowa-Housing data
and fit a predictive model based on decision trees.
