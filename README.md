# Aggregative Movie Preference Analyzer

A Python-based software system developed for the statistical analysis and exploration of movie data from the MovieLens 10M dataset. This project was developed as **Assignment 1** for the **Software Development Tools & Systems Programming (PLH 211)** course at the **Technical University of Crete** (Winter Semester 2024-2025).

## 📌 Project Overview
The objective of this assignment is to develop small-scale software for aggregative statistical analysis of user-rated movie datasets. The project focuses on applying core software engineering practices, specifically **Logging**, **Profiling**, **Refactoring**, and **Unit Testing** in a practical scenario using Python.

## 🚀 Features & Command Menu
The application features a command-line interface (CLI) where users can execute various data analysis queries:

| Command | Description |
| :--- | :--- |
| `rating T1 T2` | Finds all movies with an average rating between T1 and T2. |
| `top_movies K` | Identifies the top K movies with the highest average rating. |
| `user_pairs K` | Finds K pairs of users who have rated the same movie. |
| `dominance` | Finds movies not "dominated" by others based on both average rating and review count. |
| `iceberg K T` | Finds movies with at least K reviews and an average rating above T. |
| `top_user K` | Identifies the top K users with the most total ratings. |
| `movie_sample S` | Displays a sample (S%) of movies from every genre. |
| `similar_users Θ` | Finds user pairs with a Cosine Similarity above threshold Θ, sorted descending. |

## 🏗️ Development Lifecycle
The project was implemented in four distinct phases:

1. **Development Phase:** Initial implementation of the core logic and command processing.
2. **Logging Phase:** Implementation of a logging system to track user actions in `logme.txt` using a standardized format.
3. **Profiling Phase:** Systematic identification of memory and computational bottlenecks using Python profilers.
4. **Refactoring Phase:** Code optimization using idiomatic Python, efficient nested collections (dictionaries, tuples), comprehensions, and generators to balance execution speed and memory utilization.
5. **Unit Testing Phase:** Implementation of test cases to verify the accuracy of statistical calculations and query results.

## 🛠️ Technical Specifications
* **Language:** Python 3 (Strictly restricted to the Standard Library; no external libraries like Pandas or NumPy).
* **Development Environment:** Google Colab.
* **Dataset:** MovieLens 10M (approx. 10 million ratings, 100,000 tags, and 10,000 movies).

## 📂 Project Structure
* `ratings.dat`: UserID, MovieID, Rating, and Timestamps.
* `tags.dat`: UserID, MovieID, Tags, and Timestamps.
* `movies.dat`: MovieID, Title, and Genres.
* `PLH211_Project1_2024_2025.ipynb`: The main notebook containing the implementation, profiling results, and unit tests.
* `logme.txt`: Execution log file.

---
*Developed for the School of Electrical and Computer Engineering, Technical University of Crete.*
