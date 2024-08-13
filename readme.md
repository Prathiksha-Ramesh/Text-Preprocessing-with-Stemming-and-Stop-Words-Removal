# Text Preprocessing with Stemming and Stop Words Removal

This repository contains the source code and resources for the **Text Preprocessing with Stemming and Stop Words Removal** project. This project demonstrates various text preprocessing techniques using the Natural Language Toolkit (NLTK), focusing specifically on removing stop words and applying stemming to text data.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
  - [Text Preprocessing Steps](#text-preprocessing-steps)
- [License](#license)
- [Contact](#contact)

## Project Overview

The **Text Preprocessing with Stemming and Stop Words Removal** project covers essential text preprocessing techniques that are commonly used in Natural Language Processing (NLP) pipelines:

- **Stop Words Removal**: Filtering out commonly used words that are often insignificant in textual analysis.
- **Stemming**: Reducing words to their root form using the PorterStemmer from NLTK.

These preprocessing steps are crucial for text normalization, making it easier to analyze and process text data for various NLP tasks such as sentiment analysis, text classification, and more.

## Dataset

The project uses a famous speech delivered by Dr. APJ Abdul Kalam, which is stored in a multi-line string variable called `paragraph`. The text contains historical context, personal reflections, and visions for India's future development.

## Project Structure

- **notebook.ipynb**: The Jupyter notebook containing the complete code for text preprocessing using NLTK.
- **LICENSE**: The Apache License 2.0 file that governs the use and distribution of this project's code.
- **requirements.txt**: A file listing all the Python libraries and dependencies required to run the project.
- **.gitignore**: A file specifying which files or directories should be ignored by Git.

## Installation

To run the project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/your-repository-name.git
``` 

2. Navigate to the project directory:

``` bash 
cd your-repository-name

``` 

3. Create a virtual environment (optional but recommended):

``` bash 
python3 -m venv venv
source venv/bin/activate   # On Windows use `venv\Scripts\activate`
``` 

4. Install the required dependencies:
``` bash 
pip install -r requirements.txt
``` 

5. Run the Jupyter notebook:

``` bash 
jupyter notebook notebook.ipynb
``` 

## Usage

Text Preprocessing Steps

The notebook demonstrates various text preprocessing techniques:

- Import Libraries: The required libraries for stemming and stop words removal are imported.

``` bash 

from nltk.stem import PorterStemmer
from nltk.corpus import stopwords
import nltk
nltk.download('stopwords')
``` 
- Load the Text Data: The text data is stored in a string variable called `paragraph`, containing Dr. APJ Abdul Kalam's speech.

- Stop Words Removal: Stop words (common words that are often removed from text data) are identified and removed from the text.

``` bash 
stopwords.words('english')
stopwords.words('german')
``` 

- Stemming: The PorterStemmer is used to reduce words to their root form

``` bash 
stemmer = PorterStemmer()
stemmed_words = [stemmer.stem(word) for word in word_list]
``` 

- Sentence Tokenization: The speech is tokenized into individual sentences using NLTK's sentence tokenizer.

``` bash 
sentences = nltk.sent_tokenize(paragraph)
``` 

This sequence of steps prepares the text for further analysis or processing, which can be essential for various downstream NLP tasks.

## License
This project is licensed under the Apache License 2.0. See the `LICENSE` file for more details.

## Contact
For any inquiries or contributions, feel free to reach out or submit an issue or pull request on GitHub.





