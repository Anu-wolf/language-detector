# Language Detection Model

This project is a language detection system that can identify 22 languages based on input text. The model is trained on a dataset containing 1,000 lines per language, providing a solid foundation for accurate detection.

## Features
- Detects 22 different languages.
- Uses a Naive Bayes classifier (MultinomialNB) for language prediction.
- Utilizes the Bag of Words (BoW) model to convert text into numerical features.
- Trained on a dataset with 1,000 lines of text per language.

## Technologies Used
- **Python**: Main programming language.
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For Numerical computing.
- **scikit-learn**: Machine learning library (for CountVectorizer, Naive Bayes classifier, and data splitting).

## Dataset
The dataset used for training contains text samples from 22 languages. Each language has 1,000 lines of text, making a balanced dataset. The dataset is publicly available and can be loaded from [this source](https://raw.githubusercontent.com/amankharwal/Website-data/master/dataset.csv).

## How the Model Works
1. **Data Loading**: The dataset is loaded using `pandas` and checked for any null values.
2. **Feature Extraction**: Text data is transformed into numerical data using `CountVectorizer`, which implements a Bag of Words model.
3. **Model Training**: The dataset is split into training and testing sets, and the Multinomial Naive Bayes model is trained on the training data.
4. **Prediction**: After training, the model is used to predict the language of new text inputs provided by the user.

##Future Improvements
Expanding the dataset to include more languages and larger text.
Improving accuracy by using advanced models like Neural Networks.
Implementing a web interface for ease of user.
