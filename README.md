# Keyword Extractor App 🔑
[!image alt](https://github.com/Talha4543/Keyword-Extractor-App/blob/74528e7db949974b42ee6e5c57a1b3fab2950c63/result.PNG)

Hey there! 👋 This is a super easy-to-use tool that helps you figure out the most important words (we call them 'keywords') in any piece of text. 

Think of it like this: if you have a long article or document, this app can quickly pick out the words that really matter. It's great for understanding what the text is all about at a glance!





## Description 📝
This application extracts keywords from text documents using TF-IDF (Term Frequency-Inverse Document Frequency) vectorization. It provides a user-friendly interface to upload documents, extract keywords, and search for specific terms within the document's vocabulary. The application is built using Flask, Python, and includes a modern UI.



## Table of Contents 🗂️
1.  [Features ✨](#features-)
2.  [Tech Stack 💻](#tech-stack-)
3.  [Installation 🛠️](#installation-)
4.  [Usage 🚀](#usage-)
5.  [Project Structure 📂](#project-structure-)
6.  [Contributing 🤝](#contributing-)
7.  [License ⚖️](#license-)
8.  [Important Links 🔗](#important-links-)
9. [How to Use 💡](#how-to-use-)
10. [Footer 👣](#footer-)



## Features ✨
*   **Keyword Extraction**: Extracts top keywords from uploaded text documents using TF-IDF. 🔍
*   **Customizable N-gram**: Supports unigrams, bigrams, and up to 3-grams.
*   **Stop Word Removal**: Option to remove common English stop words to improve keyword relevance. 🚫
*   **Sensitivity Adjustment**: Adjust the score threshold to filter keywords based on relevance.
*   **Keyword Search**: Allows users to search for specific keywords within the extracted vocabulary. 🔎
*   **File Upload**: Supports uploading `.txt` files. 📤
*   **Copy/Export**: Option to copy extracted keywords or export them in JSON or CSV format. 📄
*   **Modern UI**: User-friendly interface for easy interaction.
*   **Highlighted Occurrences:** Highlights the occurrences of the keywords in the uploaded text. 🖍️



## Tech Stack 💻
*   **Backend**: Python, Flask 🐍
*   **Frontend**: HTML, CSS, JavaScript
*   **Libraries**: nltk, scikit-learn, pickle



## Installation 🛠️
1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Talha4543/Keyword-Extractor-App.git
    cd Keyword-Extractor-App
    ```
2.  **Install the required Python packages:**
    ```bash
    pip install flask nltk scikit-learn
    ```
3.  **Download necessary NLTK data:**
    ```python
    import nltk
    nltk.download('stopwords')
    nltk.download('wordnet')
    nltk.download('punkt')
    ```
4.  **Place the pickle files**
Make sure that `count_vectorizer.pkl`, `tfidf_transformer.pkl`, and `feature_names.pkl` are in the same directory as `app.py`.



## Usage 🚀
1.  **Run the Flask application:**
    ```bash
    python app.py
    ```
2.  **Open the application in your web browser** at `http://127.0.0.1:5000`.
3.  **Upload a `.txt` file** or paste text into the text area.
4.  **Adjust the settings** for n-gram, minimum word length, stop word removal, and sensitivity as desired.
5.  **Click the "Extract Keywords" button** to extract keywords from the document.
6.  **View the extracted keywords** in the results section. You can click on a keyword to highlight its occurrences in the text.
7.  **Use the Search Keywords Functionality** To search for keywords use the search keyword bar and the keywords containing the searched value will be populated
8.  **Copy or Export** Use the copy or export buttons to copy keywords or export to JSON or CSV formats.



### How to use the project in real life scenarios 🧑‍💼
**Content Analysis for SEO:**
*   **Scenario**: A digital marketing team wants to optimize website content for search engines.
*   **How to Use**: Upload webpage content (saved as .txt) to identify the most relevant keywords. Adjust n-gram settings to find key phrases. Use the results to refine SEO strategies, such as incorporating keywords into meta descriptions and headings.

**Academic Research Paper Review:**
*   **Scenario**: A researcher needs to quickly understand the key concepts in a large collection of research papers.
*   **How to Use**: Upload the abstract or main body of each paper to extract keywords. Use the
