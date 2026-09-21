# WikiKnowledge Explorer 🔎📚

WikiKnowledge Explorer is a Python-based knowledge exploration project
that works with structured Wikipedia data.

The project allows users to search and explore Wikipedia articles,
article information, entities, relationships, and other structured
content.

## 🚀 Project Overview

WikiKnowledge Explorer was originally developed to explore structured
Wikipedia knowledge using Python and Streamlit.

As part of the Wikimedia integration, the project was adapted and
tested using the **Wikimedia Structured Contents dataset** available
on Kaggle.

## 🎯 Objectives

- Explore structured Wikipedia article data.
- Search for Wikipedia articles.
- Display important article information.
- Explore entities and relationships.
- Work with Wikimedia Structured Contents data.
- Identify articles with missing or short abstracts.

## 🗂️ Wikimedia Dataset Integration

The project was integrated with the Wikimedia Structured Contents
dataset containing structured information from English Wikipedia.

The dataset is provided in **Parquet** format.

Important fields used by the project include:

- `name`
- `abstract`
- `description`
- `main_entity`
- `additional_entities`
- `references`
- `sections`
- `url`

The project was tested in a **Kaggle Notebook** using the Wikimedia
dataset.

## ✨ Features

### 🔎 Article Search

Users can search for Wikipedia articles using the article name.

The search supports:

- Exact article matches
- Partial article matches
- Word-based exploration

### 📄 Article Information

The project displays structured information about selected articles,
including:

- Article name
- Description
- Abstract
- Main entity
- Language
- Wikipedia URL

### 🔗 Relationships

The project can explore relationships between articles and entities
using structured Wikimedia information.

### 🧩 Dataset Exploration

The project provides information about the dataset and its available
structured fields.

### 🆕 Weak Article Finder

A new feature was added during the Wikimedia integration.

The Weak Article Finder identifies articles whose abstracts are:

- Missing, or
- Less than 100 characters long.

This feature provides a simple way to identify articles that may
require further abstract-quality inspection.

## 🛠️ Technologies Used

- Python
- Pandas
- Streamlit
- Regular Expressions
- Parquet
- Wikimedia Structured Contents
- Kaggle

## 📊 Testing

The project was tested using the Wikimedia Structured Contents
dataset in Kaggle.

During testing:

- Wikimedia Parquet files were successfully loaded.
- Article search functionality was tested.
- Structured article information was retrieved.
- The Weak Article Finder was implemented and tested.
- One Wikimedia English Wikipedia namespace-0 shard containing
  approximately 25,000 articles was used for the demonstration.

The tested shard contained **4,998 articles with missing or short
abstracts** using the project's `<100 character` criterion.

## 📁 Project Structure

```text
WikiKnowledge-Explorer/
│
├── app.py
├── requirements.txt
└── README.md
