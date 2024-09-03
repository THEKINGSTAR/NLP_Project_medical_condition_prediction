# Disease Condition Prediction Based on Drug Reviews

## ```Project Overview```

This project focuses on predicting the medical conditions of patients based on their drug reviews. By analyzing the textual content of the reviews, we aim to classify the condition that the patient is likely experiencing. This project utilizes the drug reviews dataset available from the UCI Machine Learning Repository.

### ```Objectives```:

- **Text Classification**: Develop a machine learning model to classify patient conditions based on the reviews they have written about the drugs they have used.
- **Natural Language Processing (NLP)**: Apply NLP techniques to preprocess and vectorize the textual data from drug reviews.
- **Model Deployment**: Deploy the trained model as a web application, allowing users to input drug reviews and predict the associated medical conditions.

## ```Repository Structure```

```plaintext
.
├── app.py                              # Flask application to run the web interface
├── data                                
│   ├── drugsComTrain.csv               # Dataset used for training the model
│   └── test                            # Directory for test data (currently empty)
├── model                               
│   ├── passmodel.pkl                   # Trained model for predicting medical conditions
│   ├── test                            # Directory for test models (currently empty)
│   └── tfidfvectorizer.pkl             # TF-IDF vectorizer used to transform textual data
├── NLP Project (Medical condition prediction).ipynb
│                                       # Jupyter Notebook documenting the project workflow
├── NLP-Project.pptx                    # Presentation summarizing the project
├── README.md                           # Project documentation
├── static                              # Static files (CSS, images)
│   └── css
│       ├── main.css                    # Main CSS file for styling the web interface
│       ├── test.txt                    # Test text file (may be used for development purposes)
│       ├── text-analysis.png           # Image related to text analysis
│       └── util.css                    # Utility CSS file for additional styling
└── templates                           # HTML templates for the Flask app
    ├── home.html                       # Home page of the web application
    ├── login.html                      # Login page for the web application
    └── predict.html                    # Page for entering reviews and predicting conditions
```

## ```Project Details```

### ```Data Source```

The dataset used for this project is the **Drug Review Dataset** from the UCI Machine Learning Repository. It contains patient reviews for various drugs along with the condition they are being treated for, providing a rich source of data for condition classification.

### ```Steps Involved```:

1. **Data Preprocessing**:
   - Load and clean the dataset.
   - Preprocess the text data (e.g., tokenization, stopword removal).
   - Transform the text data into numerical features using TF-IDF vectorization.

2. **Model Training**:
   - Train a classification model using the processed data.
   - Evaluate the model's performance using appropriate metrics.

3. **Model Deployment**:
   - Save the trained model and vectorizer for future use.
   - Develop a Flask web application that allows users to input drug reviews and receive predictions about the associated medical conditions.

4. **Web Application**:
   - The app.py script runs a Flask web application where users can interact with the model.
   - The application consists of multiple pages, including a home page, login page, and prediction page.

### ```Running the Project```

To run the web application locally, follow these steps:

1. **Clone the Repository**: Download the project files to your local machine.
2. **Install Dependencies**: Make sure you have Python installed, then install the required packages using:
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the Application**: Start the Flask web application by running:
   ```bash
   python app.py
   ```
4. **Access the Application**: Open your web browser and navigate to `http://localhost:5000` to use the application.

## ```Additional Resources```

- **[NLP Project Notebook](NLP%20Project%20(Medical%20condition%20prediction).ipynb)**:  
  Explore the detailed Jupyter Notebook documenting the entire project workflow, from data preprocessing to model training and evaluation.

- **[Project Presentation](NLP-Project.pptx)**:  
  View the presentation summarizing the key aspects of the project.

## ```Acknowledgments```

This project was developed as part of an academic requirement at Alexandria University, under the guidance of the Department of Information Technology.