# Email Spam Detection Dataset

## Dataset Overview
This dataset contains preprocessed email data for spam/not-spam classification. The dataset consists of 5,172 randomly selected email files that have been transformed into a structured format suitable for machine learning applications.

## Dataset Structure

### File Information
- **Format**: CSV (Comma-Separated Values)
- **Total Rows**: 5,172 (one per email)
- **Total Columns**: 3,002
- **File Size**: Compact representation of 5,172 individual email files

### Column Description

#### Column 1: Email Name
- **Type**: Identifier
- **Format**: Numeric identifiers (anonymized)
- **Purpose**: Unique identification for each email
- **Privacy**: Original recipient names replaced with numbers for privacy protection

#### Columns 2-3001: Word Frequency Features
- **Type**: Numeric (Integer counts)
- **Description**: Count of each word occurrence in the corresponding email
- **Feature Set**: 3,000 most common words across all emails
- **Preprocessing Applied**:
  - Non-alphabetical characters excluded
  - Non-alphabetical words removed
  - Word frequency counts calculated for each email

#### Column 3002: Label
- **Type**: Binary classification target
- **Values**: 
  - `1` = Spam email
  - `0` = Not spam (legitimate email)

## Data Characteristics

### Dataset Dimensions
- **Total Emails**: 5,172
- **Feature Dimensions**: 3,000 word features
- **Data Type**: Word count matrix (bag-of-words representation)
- **Sparsity**: High (most emails contain only a subset of the 3,000 words)

### Data Processing
The original email text files have been converted into a structured format where:
- Each row represents one email
- Each column (2-3001) represents the count of a specific word in that email
- The 3,000 words were selected as the most frequently occurring words across all emails
- All non-alphabetical content has been filtered out

## Dataset Summary
This dataset provides a compact, privacy-protected representation of email data suitable for spam classification tasks. The word count matrix format allows for efficient storage and processing while maintaining the essential information needed for text classification algorithms.
