# AI-Based Sentiment Analysis Application

This repository contains an AI-based sentiment analysis application built using IBM Watson NLP embedded libraries. The application is designed to analyze the sentiment of textual data, providing insights into the emotions and opinions expressed within the text. It is packaged for easy integration into any Python project and is deployed as a web service using the Flask framework.

## Features

- **Sentiment Analysis:** Leverages Watson NLP embedded libraries to analyze and extract sentiment from textual data.
- **Formatted Output:** The output from the Watson NLP library function is processed to extract and present relevant information in a user-friendly format.
- **Reusable Package:** The application is packaged and can be imported into any Python project, making it easy to integrate sentiment analysis functionality.
- **Unit Testing:** Comprehensive unit tests have been implemented to validate the accuracy and robustness of the sentiment analysis for different input scenarios.
- **Flask Deployment:** The application is deployed as a web service using Flask, allowing for easy access and interaction via HTTP requests.
- **Error Handling:** The application includes robust error handling, ensuring that a response code of 500 triggers an appropriate response from the application.
- **PEP8 Compliance:** Static code analysis has been performed to ensure that the code adheres to PEP8 guidelines, ensuring readability and maintainability.

## Installation

To use this application, clone this repository and install the required dependencies:

```bash
git clone URL
cd sentiment-analysis-app
pip install -r requirements.txt
```

## Usage

### As a Python Package

You can import the sentiment analysis functionality into your own Python projects:

```python
from sentiment_analysis import analyze_sentiment

text = "This is an example text to analyze."
result = analyze_sentiment(text)
print(result)
```

### As a Web Service

Run the Flask server to deploy the application as a web service:

```bash
flask run
```

Send a POST request with the text you want to analyze:

```bash
curl -X POST http://localhost:5000/analyze -d "text=This is an example text to analyze."
```

The response will include the analyzed sentiment and other relevant information.

## Testing

To run the unit tests and verify the application’s functionality:

```bash
pytest
```

## Error Handling

The application handles errors gracefully. In the event of a server error (HTTP 500), the application will return a meaningful error message along with the status code.

## Code Quality

The code has been analyzed for PEP8 compliance. To run static code analysis:

```bash
flake8 .
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributions

Contributions are welcome! Please fork this repository and submit a pull request with your changes.

## Contact

For any questions or issues, please open an issue in the repository or contact the project maintainer at bouhali.hamza.2@gmail.com.
