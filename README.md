# -Financial-Data-Deduplication-Tool
A Python-based MVP designed for lean investment banking teams to automate CRM hygiene. Utilizing fuzzy-logic string matching (Levenshtein distance), this tool identifies "near-match" duplicates, like typos and abbreviations, that standard filters miss. Features a dynamic Streamlit UI for threshold-based data cleaning.

An AI-driven solution for cleaning messy CRM contact records in lean deal environments.

The Problem
Frontline staff often waste hours manually identifying duplicate records due to typos, abbreviations (e.g., "Corp" vs "Corporation"), or inconsistent punctuation.

The Solution
This tool uses **Fuzzy-Logic String Matching** (Levenshtein Distance) to identify "near-match" duplicates that standard database filters miss. 

Key Features:
Similarity Scoring: Quantifies how close two names are on a scale of 0-100.
Dynamic Thresholding: A slider-based UI to control sensitivity vs. precision.
Token Sorting: Handles word re-ordering (e.g., "Advisors Birch Creek" vs "Birch Creek Advisors").

Tech Stack
Language: Python
Interface: Streamlit
Core Logic: TheFuzz (FuzzyWuzzy) / Pandas
