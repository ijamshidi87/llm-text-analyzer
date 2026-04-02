# LLM Text Analyzer

A Google Colab notebook that analyzes text files and computes linguistic metrics using spaCy.

## What It Does

Upload one or more `.txt` files (e.g., LLM responses) and get an Excel file with:

| Column | Description |
|---|---|
| Scenario ID | Name of the uploaded `.txt` file (without extension) |
| Word Count | Total number of words |
| Sentence Count | Total number of sentences |
| average_sentence_length | Average number of words per sentence |

## How to Use

1. Open the notebook in Google Colab
2. Run **Cell 1** to install dependencies (`spaCy`, `openpyxl`)
3. **Restart the runtime** (Runtime → Restart session)
4. Run **Cell 2** to upload your `.txt` files
5. Run **Cell 3** to analyze the files — a preview table will appear
6. Run **Cell 4** to download `results.xlsx`

> ⚠️ After installing spaCy for the first time, you must restart the runtime before proceeding to Cell 2.

## Requirements

No local installation needed — runs entirely in Google Colab.

| Package | Purpose |
|---|---|
| spaCy (`en_core_web_sm`) | Sentence and word tokenization |
| openpyxl | Excel file generation |
| pandas | Data preview in notebook |

## Input Format

- Plain text files (`.txt`)
- English text
- File name = Scenario ID (e.g., `H1.txt` → `H1`)

## Output

An Excel file (`results.xlsx`) with one row per uploaded file and color-coded formatting.
