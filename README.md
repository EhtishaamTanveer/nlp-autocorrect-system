# Autocorrect System - Natural Language Processing

This repository contains an implementation of an autocorrect system using Natural Language Processing (NLP) techniques. It's designed to suggest corrections for misspelled words based on word frequencies in a given corpus and string manipulation techniques.

## Project Overview

This project implements an autocorrect system that suggests corrections for misspelled words. It uses a text corpus to calculate word probabilities and employs string manipulation techniques to generate possible corrections. The minimum edit distance algorithm ([Levenshtein distance](https://en.wikipedia.org/wiki/Levenshtein_distance)) is used to further refine suggestions by calculating the minimum number of edits (insertions, deletions, substitutions) required to transform one word into another.

## Key Features

*   **Data Preprocessing:** Tokenization, counting word occurrences, and calculating word probabilities from a given text corpus.
*   **String Manipulation:** Generating candidate corrections using operations like deleting, switching, replacing, and inserting letters.
*   **Edit Distance Calculation:** Utilizing dynamic programming to efficiently compute the minimum edit distance between words.
*   **Spelling Suggestions:** Ranking and providing the most probable spelling suggestions based on word probabilities and edit distance.
*   **Modular Design:** The code is organized into functions for better readability, maintainability, and reusability.
*   **Example Usage and Demonstration:** A Jupyter Notebook provides a clear demonstration of how to use the autocorrect system.

## Usage

### Running the Script Directly:

-  Place your text corpus in the `data/` directory. By default the code looks for `data/shakespeare.txt`. You can change this according to your needs.
-  Open nlp-autocorrect.ipynb (The notebook guides you through the functionalities of the autocorrect system)


## File Structure

* nlp-autocorrect.ipynb: main project jupyter notebook.
* w1_unittest.py: contains all the test cases which are used to check the functions in the main notebook.
* data/
  * shakespeare.txt: file containing the corpus used to build the autocorrect system
* README.md: this file


## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request to improve this project.
