# Evaluating Large Language Models in Categorization Task
This project evaluates GPT's ability to categorize words by similarity. "Categorization" refers to the mental process of sorting objects or ideas into categories or groups based on shared features, properties, or relationships. It relies on general knowledge and understanding of the world to identify similarities and differences among items and organize them accordingly. This project aims to see how well GPT models, GPT-2 and GPT-3.5, can categorize words using past New York Times' Connections games, which with its diverse words and categories, encompasses different types of categorization. Additionally, given the different difficulty levels of categories, the project will see how well GPT perform versus New York Times' expected human performance on certain difficulty levels. This gives us some insight into how closely LLM's ability to categorize is to humans' ability to categorize.

## Overview

### Usage

First, use the `script.py` file as a querying method. All results will be saved into a `answers.csv` or `prompts.csv` as seen in `connections-pilot.ipynb`.

Options:

-  `-d`, `--debug`: Writes to the log dir

-  `-s`, `--serialize`: Serializes the raw HTML for ad hoc analysis

  

Next, you can generate the `results-2.csv` or `results-3.csv` as demonstrated in `analysis.ipynb`.

### Tech Stack

Web querying is handled by Selenium using a head based Chromium browser. There is an option to use the `requests` package in place of Selenium. GPT-3.5 responses collected from OpenAI's Python library, and GPT-2 reponses collected Hugging Face's Transformers library. Core language is in Python.
