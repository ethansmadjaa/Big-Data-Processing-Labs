# Final Project - Big Data Processing

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Apache%20Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![uv](https://img.shields.io/badge/uv-DE5FE9?style=for-the-badge&logo=uv&logoColor=white)

[![GitHub](https://img.shields.io/badge/GitHub-ethansmadjaa-181717?style=flat-square&logo=github)](https://github.com/ethansmadjaa)

---

## Description

Final project for the **Big Data Processing** course at ECE Paris. This project meets the requirements defined in [Final Project.md](Final%20Project.md).

---

## Authors

| Name             | Role    |
| ---------------- | ------- |
| **Ethan Smadja** | Student |
| **Tom Urban**    | Student |

---

## Project Content

The project consists of two complementary notebooks:

### 1. IMDB Analysis (`IMDB_ANALYSIS.ipynb`)

Complete analysis of IMDB data answering the following questions:

- Total number of people in the dataset
- Oldest birth year
- Validation of birth dates
- Most recent birth date
- Percentage of people without a birth date
- Duration of the longest "short" after 1900
- Duration of the shortest "movie" after 1900
- List of all represented genres
- Highest-rated comedy film
- Director and alternative titles of the film

### 2. Stream Processing (`streaming.ipynb`)

Real-time stream processing with the Wikimedia EventStreams API:

- **Tracked Entities**: Christopher Nolan, The Godfather, Quentin Tarantino, Science Fiction, Academy Awards
- **Fuzzy Matching with Levenshtein Distance**:
  - Uses `python-Levenshtein` library for efficient string similarity
  - Threshold set at **0.80** (80% similarity required for a match)
  - Enables matching of page title variations (typos, formatting differences)
  - Each matched event includes a `match_score` field (1.0 = exact match)
- **Real-time Metrics Collection**:
  - Total edits per entity
  - Bot vs human edit classification
  - Bytes changed tracking
  - Unique users tracking
- **Alert System**:
  - Large edits (>500 bytes changed)
  - Bot edit detection
  - Rapid successive edits (potential edit wars)
- **Data Storage** in JSON files:
  - `streaming_output/wiki_events.json` - All captured events
  - `streaming_output/wiki_alerts.json` - Alert events
  - `streaming_output/metrics_summary.json` - Aggregate metrics

---

## Execution

> To run the notebooks, simply click **"Run All"** and you're good to go!

---

## Acknowledgments

Many thanks to the professor for this enriching course on Big Data Processing.

---

<p align="center">
  <i>ECE Paris - Big Data Processing</i>
</p>