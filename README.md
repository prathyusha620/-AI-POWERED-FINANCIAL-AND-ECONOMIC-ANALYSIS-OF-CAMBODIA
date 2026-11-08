# -AI-POWERED-FINANCIAL-AND-ECONOMIC-ANALYSIS-OF-CAMBODIA


AI-Powered Financial and Economic Analysis of Cambodia

The following is a list of features included with our software: PDF-based information extraction, AI summarization, retrieval-augmented generation and dashboard visualization.

Project Overview

This project will create a pipeline that uses artificial intelligence to collect, summarize, evaluate, and present the financial and economic data found in the International Monetary Fund (IMF) Country Report for Cambodia (IMF Country Report No. 24/36, 2024).

This is a project that utilizes Python on Google Colab to take a long-form PDF report, process it through large language models (LLMs), natural language processing (NLP), semantic searches, and data visualizations, so that you can turn it into structured economic insight and an interactive analysis dashboard.

Student: P. Sudireddy

Student ID: 24158287

Country: Cambodia

Source: IMF Country Report No. 24/36

Objectives

Extract and preprocess text from the IMF PDF report.

Apply token-aware chunking for efficient AI processing.

Generate executive and thematic summaries using Google Gemini.

Evaluate AI-generated summaries to ensure they are factually accurate, comprehensive and consistent.

Extract financial indicators and classify economic evidence.

Identify economic and financial strengths and weaknesses.

Implement a Retrieval-Augmented Generation (RAG) system.

Develop a four-panel economic and financial dashboard.

Technologies Used

Python and Google Colab: Development environment.

PyPDF: PDF text extraction.

Tiktoken: Tokenisation and text chunking.

Google Gemini 3.8 Flash: AI summarisation and information extraction.

Pandas and NumPy: Data processing and analysis.

Sentence Transformers: Semantic text embeddings.

all-MiniLM-L6-v2: 384-dimensional embedding model.

FAISS: Vector indexing and similarity search.

Matplotlib: Data visualisation.

JSON: Structured data storage.

Methodology

I processed the 114 pages of the IMF report with PDF extraction and cleaning of the text to produce about 233,313 characters and 35,421 words.

The 177 segments that were pulled from the document were processed by Gemini in 12 separate groups to create executive and thematic summaries. To do so, each segment used a 400-token size, with a 50-token overlap between segments.

The project categorized 253 passages into seven economic topics and extracted significant financial metrics. A local RAG system was built with Sentence Transformers and FAISS, which retrieved the top five most pertinent document segments for user searches.

Key Results

177 processed text chunks.

253 thematically classified passages.

7 economic and financial categories.

9.1/10 overall AI-assisted summary evaluation score.

4 dashboard visualisations.

384-dimensional semantic embeddings.

Indicators such as GDP growth at 5.3% (as of 2023), headline inflation at 3.9% (as of October 2023), non-performing loan ratio at 4.6% (as of August 2023), and Tier 1 Capital Ratio at 18.8% (as of 2022) were extracted.

Dashboard

The final dashboard presents four visualisations:

Thematic distribution of economic evidence.

Inflation trends and monetary conditions.

AI summary evaluation results.

Private credit growth compared with non-performing loan ratios.

Installation

Install the required dependencies:

pip install pypdf tiktoken pandas numpy matplotlib sentence-transformers faiss-cpu google-genai

Start by opening your Jupyter Notebook in Google Colab. Then run each cell one-after-the-other. To process data with an AI, you will need to obtain access to the Gemini API. You may store your API key in either Colab Secrets or as an Environment Variable.

Limitations

Human verification is required on all AI generated outputs compared to the original IMF report. The evaluation process utilized the same Gemini model but a separate evaluation prompt. Several indicators such as the Central Bank Policy Rate and Unemployment Rate were missing from the extracted source data.

Data Source

The International Monetary Fund (2024). Cambodia: 2023 Article IV Consultation - Press Release and Staff Report. IMF Country Report No. 24/36.

View the IMF Report

Academic project – University of Hertfordshire.
