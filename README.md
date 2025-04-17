# Umesh Chandra - NLP Processing and Analysis Pipeline

## 1. NLP Preprocessing Pipeline Overview

### Example Output:
For input: "NLP techniques are used in virtual assistants like Alexa and Siri."


1. **Original Tokens**:  
`['NLP', 'techniques', 'are', ..., 'Siri', '.']`

2. **After Removing Stopwords**:  
`['NLP', 'techniques', 'used', ..., 'Alexa', 'Siri']`

3. **Stemmed Tokens**:  
`['nlp', 'techniqu', 'use', ..., 'alexa', 'siri']`

### Key Notes:
- Requires NLTK data packages (`punkt`, `stopwords`).
- Stemming may generate non-standard words (trade-off for simplicity and speed).

---

## 2. Named Entity Recognition (NER) Overview

### Key Features:
- Leverages spaCy's `en_core_web_sm` model for entity recognition.
- Extracts entities and includes:
  - Entity text content
  - Entity type (e.g., PERSON, DATE)
  - Character position indices in the text.

### Example Output:
For input: "Barack Obama served as the 44th President..."

Entities Detected:
- `Barack Obama` (PERSON) [0:12]
- `the 44th` (ORDINAL) [21:28]
- `the United States` (GPE) [39:54]
- `the Nobel Peace Prize` (WORK_OF_ART) [64:84]
- `2009` (DATE) [88:92]

### Important Notes:
- Requires spaCy and the English language model.
- Pre-trained model detects common entity types.
- Character position tracking allows for easy text highlighting or further analysis.

---

## 3. NLP Processing Pipeline on GitHub

### 1. NLP Preprocessing Pipeline

#### Key Components:
- **Tokenization**: Uses NLTK's `word_tokenize` for splitting text into words.
- **Stopword Removal**: Removes common, non-informative English words.
- **Porter Stemming**: Applies stemming to reduce words to their root form.

### 2. Named Entity Recognition (NER)

#### Core Features:
- Uses spaCy’s pre-trained English model to identify named entities.
- Extracts entities with labels and tracks their positions in the text.
- Supports detecting entities like PERSON, DATE, GPE, and WORK_OF_ART.

### 3. Scaled Dot-Product Attention

#### Core Features:
- Implements the attention mechanism from Transformer models.
- Computes the scaled dot-product of Query and Key matrices: `Q·Kᵀ / √d`.
- Applies softmax to calculate attention weights.
- Generates output as a weighted sum of the Value matrix.

---

## 4. Sentiment Analysis Overview

### Key Features:
- Uses Hugging Face's `transformers` pipeline for sentiment analysis.
- Pre-trained model returns the sentiment label (POSITIVE or NEGATIVE) along with a confidence score.

### Main Highlights:
- **Zero-shot classification**: No additional training needed.
- Handles complex and nuanced sentiments (e.g., mixed or neutral statements).
- Higher confidence scores indicate stronger sentiment predictions.

---

Entities Detected:
- `Barack Obama` (PERSON) [0:12]
- `the 44th` (ORDINAL) [21:28]
- `the United States` (GPE) [39:54]
- `the Nobel Peace Prize` (WORK_OF_ART) [64:84]
- `2009` (DATE) [88:92]

### Important Notes:
- Requires spaCy and the English language model.
- Pre-trained model detects common entity types.
- Character position tracking allows for easy text highlighting or further analysis.

---

## 3. NLP Processing Pipeline on GitHub

### 1. NLP Preprocessing Pipeline

#### Key Components:
- **Tokenization**: Uses NLTK's `word_tokenize` for splitting text into words.
- **Stopword Removal**: Removes common, non-informative English words.
- **Porter Stemming**: Applies stemming to reduce words to their root form.

### 2. Named Entity Recognition (NER)

#### Core Features:
- Uses spaCy’s pre-trained English model to identify named entities.
- Extracts entities with labels and tracks their positions in the text.
- Supports detecting entities like PERSON, DATE, GPE, and WORK_OF_ART.

### 3. Scaled Dot-Product Attention

#### Core Features:
- Implements the attention mechanism from Transformer models.
- Computes the scaled dot-product of Query and Key matrices: `Q·Kᵀ / √d`.
- Applies softmax to calculate attention weights.
- Generates output as a weighted sum of the Value matrix.

---

## 4. Sentiment Analysis Overview

### Key Features:
- Uses Hugging Face's `transformers` pipeline for sentiment analysis.
- Pre-trained model returns the sentiment label (POSITIVE or NEGATIVE) along with a confidence score.

### Main Highlights:
- **Zero-shot classification**: No additional training needed.
- Handles complex and nuanced sentiments (e.g., mixed or neutral statements).
- Higher confidence scores indicate stronger sentiment predictions.

---


