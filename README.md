> **I'm back to make you laugh, 'cause this repo won't do that.**
> 
> **Why do cows wear bells?**  
> *Because their horns don’t work.*


IndiTranslate (Poster Text Translation Project)

This project translates text on posters into regional languages and maps the translated text back onto the posters, creating localized versions of visual materials. The tool utilizes advanced image processing techniques combined with natural language processing (NLP) to detect, translate, and remap text.

Features

	•	Text Detection: Extracts text from images or posters.
	•	Translation: Converts the extracted text into regional languages.
	•	Text Mapping: Maps the translated text back onto the original image, replacing the detected text.

Project Structure

	•	main.py: Contains the main logic for the project, including the text extraction and translation workflow.
	•	image.py: Handles image-related processing tasks, including text detection and mapping translated text back onto the poster.

Requirements

Before running the project, you need to have the following dependencies installed:

	•	Python 3.x
	•	OpenCV
	•	pytesseract
	•	Google Cloud Translate API (or an alternative translation API)
	•	NumPy
	•	PIL (Pillow)

You can install the required packages using pip:

pip install opencv-python pytesseract google-cloud-translate numpy Pillow

Additional Setup

You may need to install Tesseract for text detection. Follow the instructions to install it based on your operating system:

	•	macOS:

brew install tesseract


	•	Ubuntu:

sudo apt-get install tesseract-ocr


	•	Windows: Download the Tesseract installer from here.

How to Use

	1.	Clone the repository:

git clone https://github.com/qamarali01/IndiTranslate
cd IndiTranslate


	2.	Prepare the Input Image:
	•	Place the image of the poster you want to translate in the project directory.
	3.	Run the script:

python main.py --image poster.jpg --lang hi

	•	Replace poster.jpg with the name of your poster image file.
	•	Use the --lang argument to specify the target regional language (for example, hi for Hindi, bn for Bengali).

	4.	View the Translated Poster:
	•	The output image with the translated text mapped back onto the poster will be saved in the project directory.

Example

Input:

	•	A poster image in English with the text “Health Camp”.

Output:

	•	The translated poster with “स्वास्थ्य शिविर” in Hindi, replacing the original English text.

Customization

	•	Translation API: By default, the project uses the Google Cloud Translate API for translation. You can switch to another service by modifying the API integration in the code.
	•	Regional Languages: The script supports all languages supported by the translation API you are using. Simply pass the desired language code as a parameter.

Contributing

If you’d like to contribute to this project, feel free to open issues or submit pull requests. Contributions such as improving the accuracy of text detection, supporting additional languages, or enhancing the mapping algorithm are welcome.


Contact

For any questions or support, feel free to contact me:

	•	Email: qamarali9584@gmail.com
	•	GitHub: github.com/qamarali01
