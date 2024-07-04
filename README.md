# Resume Match

## Resume Similarity Checker with Streamlit

This repository provides a Streamlit application to calculate the cosine similarity between two uploaded documents for plagiarism or job fit assessment.

The app is deployed on streamlit server and can be run at: 
[Resume Match - A Streamlit app](https://share.streamlit.io/kashifm777/resumematch/main/ResumeMatch.py)

### 1. Features

- **Cosine Similarity:** Compares two uploaded documents (PDF format) to determine the level of textual similarity. 
- **Intuitive Interface:**  A user-friendly interface with clear instructions and separate sections for Home and Check Similarity functionalities.
- **File Upload:** Upload both your resume and the job description (or any two documents) for comparison. 
- **Similarity Score:** Displays the calculated cosine similarity score as a percentage, indicating the level of textual match between the documents.

### 2. Requirements

- Python 3.x
- Streamlit (`pip install streamlit`)
- PyPDF2 (`pip install PyPDF2`)
- scikit-learn (`pip install scikit-learn`)

### 3. Running the App

1. Ensure you have Python and the required libraries installed.
2. Open a terminal in the project directory.
3. Run the app: `streamlit run main.py` (replace `main.py` with the actual name of your main Python file if it's different)
4. Access the app in your web browser at http://localhost:8501

### 4. How it Works

1. The application utilizes the Streamlit framework for a user-friendly web interface.
2. Users can navigate between "Home" and "Check Similarity" sections using the sidebar menu.
3. In the "Check Similarity" section, upload both your resume and the job description (or any two documents) in PDF format.
4. Clicking the "Check Similarity" button triggers the comparison process.
5. The application utilizes PyPDF2 to extract text content from both uploaded documents.
6. It then preprocesses the text using CountVectorizer from scikit-learn to create a numerical representation of the documents.
7. Finally, the cosine similarity between the two documents is calculated and displayed as a percentage, indicating the level of textual match.

### 5. Note

- This is a basic implementation for demonstration purposes. 
- Consider adding support for additional document formats (e.g., docx, txt) in the future.
- Explore more sophisticated text preprocessing techniques for improved accuracy.

### 6. Further Enhancements

- Implement text cleaning and normalization techniques before similarity calculation.
- Provide the option to upload a single document and compare it against a reference document.
- Display a visual representation of the similarity score (e.g., bar chart).
