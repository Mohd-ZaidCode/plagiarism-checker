# Plagiarism Checker - Console Application
This console application is a basic plagiarism checker built using Python. It utilizes the sklearn library for vectorization and cosine similarity computation and the tkinter library for selecting a directory containing text files to check for plagiarism.

## Requirements
Python 3.x
numpy library (can be installed using pip install numpy)
scikit-learn library (can be installed using pip install scikit-learn)
tkinter library (should be pre-installed with Python)
## Usage
Clone the repository or download the code files.
Install the required dependencies using the command pip install -r requirements.txt.
Run the plagiarism_checker.py file using the command python plagiarism_checker.py.
The application will prompt you to select a directory containing the text files to check for plagiarism.
After selecting the directory, the application will process the files and display pairs of files that potentially contain plagiarized content, along with their similarity scores.
## How it works
The Addmusic function uses the tkinter library to prompt the user to select a directory containing the text files to check for plagiarism. It returns a list of file names ending with .txt.

The application then reads the contents of each selected file and stores them in the sample_contents list.

The vectorize function uses TfidfVectorizer from sklearn to convert the text data into numerical vectors using the Term Frequency-Inverse Document Frequency (TF-IDF) algorithm.

The similarity function uses cosine_similarity from sklearn to compute the cosine similarity between two given vectors.

The vectors variable stores the numerical vectors obtained from the text contents of the files.

The s_vectors variable pairs each file with its corresponding vector.

The check_plagiarism function iterates through each file and compares it with the other files, calculating the similarity scores using cosine similarity.

The results are stored in a set to avoid duplicates and printed to the console.

## Screenshot

![image](https://github.com/Mohd-ZaidCode/plagiarism-checker/assets/127447741/3be48fcc-24d7-42ca-a289-c1cc1d1e8d45)

