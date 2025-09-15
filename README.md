# Scientific Keyphrase Extractor 🔑🔬

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://skeforu.streamlit.app/)

A powerful web application built with Streamlit that uses Natural Language Processing (NLP) to analyze scientific documents (`.pdf` and `.docx`) and extract the most relevant keyphrases. It features a secure user authentication system and presents the results through a suite of stunning, interactive visualizations.

### ➡️ **[View the Live Demo](https://skeforu.streamlit.app/)**

---

## ✨ Key Features

* 🔐 **Secure User Authentication**: A complete registration and login system with password hashing (`PBKDF2HMAC`) and salting to protect user data.
* 📁 **Multi-Format Document Support**: Seamlessly upload and process both `.pdf` and `.docx` files.
* 🧠 **Advanced NLP Core**: Utilizes the **TF-IDF** (Term Frequency-Inverse Document Frequency) algorithm to intelligently identify, score, and rank the most significant phrases (from unigrams to trigrams).
* 📊 **Rich Interactive Visualizations**:
    * **Word Cloud**: A dynamic visual representation of keyphrase prominence.
    * **Donut Chart**: Understand the proportional importance of each keyphrase at a glance.
    * **Radial Bar Chart**: A unique and beautiful chart mapping keyphrase frequency and importance.
    * **Frequency Histogram**: A classic bar chart for easily comparing term frequencies.
* 🎛️ **Customizable Analysis**: An intuitive slider allows you to select the exact number of top keyphrases you want to analyze.
* 📜 **Persistent Activity History**: Your past analyses are saved to your account. You can revisit any previous document's keyphrases and visualizations at any time.

---

## 🚀 Visual Showcase

Here's a glimpse of the extractor in action, transforming a dense document into insightful visualizations.


| Word Cloud | Donut Chart | Radial Chart |
| :---: | :---: | :---: |
| *Visualize term importance* | *Compare proportional relevance* | *See frequency in a unique layout* |
|  |  |  |

---

## 🛠️ Tech Stack

This project is built with a modern, robust stack:

* **Backend & Frontend**: [Streamlit](https://streamlit.io/)
* **NLP/Data Manipulation**: [Scikit-learn](https://scikit-learn.org/), [Pandas](https://pandas.pydata.org/), [NumPy](https://numpy.org/)
* **Data Visualization**: [Matplotlib](https://matplotlib.org/), [Seaborn](https://seaborn.pydata.org/), [WordCloud](https://github.com/amueller/word_cloud)
* **File Processing**: [PyPDF2](https://pypdf2.readthedocs.io/), [python-docx](https://python-docx.readthedocs.io/)
* **Database**: `SQLite3` (Python Standard Library)
* **Security**: `Cryptography` library for hashing and encryption.

---

## ⚙️ Getting Started

To run this project on your local machine, follow these simple steps.

### Prerequisites

* Python 3.8+
* `pip` package manager

### Installation & Setup

1.  **Clone the Repository**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
    cd YOUR_REPOSITORY_NAME
    ```

2.  **Create and Activate a Virtual Environment**
    * **On macOS/Linux:**
        ```bash
        python3 -m venv venv
        source venv/bin/activate
        ```
    * **On Windows:**
        ```bash
        python -m venv venv
        .\venv\Scripts\activate
        ```

3.  **Install Dependencies**
    The `requirements.txt` file contains all necessary packages.
    ```bash
    pip install -r requirements.txt
    ```

4.  **Run the Streamlit App**
    Once the dependencies are installed, you can launch the application.
    ```bash
    streamlit run app.py
    ```
    Your web browser should automatically open to the app's local address (`http://localhost:8501`).

---

## Usage Guide

1.  **Register/Login**: Create a new account or log in with existing credentials.
2.  **Upload File**: Drag and drop (or browse for) a `.pdf` or `.docx` file.
3.  **Set Keyphrase Count**: Use the slider to define how many top keyphrases you'd like to extract.
4.  **Extract**: Click the "Extract Keyphrases" button to begin the analysis.
5.  **Explore**: View the results in the data table and the interactive plots that appear below.
6.  **Review History**: Scroll down to the "Your Past Activities" section to expand and revisit any of your previous analyses.

---

## 🤝 Contributing

Contributions are welcome! If you have suggestions for improvements or want to add new features, feel free to fork the repository, create a new branch, and submit a pull request.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

---

## 📄 License

This project is distributed under the MIT License. See the `LICENSE` file for more information.
