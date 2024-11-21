# auto-generation-of-distictive-features

Overview
The IPA Feature Lookup Tool is a simple and efficient application designed to help linguists, researchers, and language enthusiasts retrieve the distinctive phonological features of any IPA (International Phonetic Alphabet) phone. Users can input an IPA symbol, and the app will instantly display its associated features, such as consonantal, sonorant, voice, nasal, and more.

Features
Fast Lookup: Input an IPA phone and retrieve its phonological features in seconds.
User-Friendly Interface: A graphical interface built with Tkinter makes the app easy to use.
Comprehensive Dataset: Covers a wide range of IPA symbols with detailed features.
Error Handling: Displays a warning if a phone is not found in the dataset.
How It Works
Input an IPA Phone: Type any IPA symbol into the input box.
View Features: Click the "Lookup" button to see the phonological features displayed in a popup message.
Error Notification: If the input phone isn't in the dataset, you'll receive a clear warning.
Example Input and Output
Input: b
Output:
diff
Copy code
+consonantal, -sonorant, +voice, -nasal, +labial, -dorsal, -coronal
Installation
Prerequisites
Python 3.6 or higher
Tkinter (usually pre-installed with Python)
pandas (if loading data from a file)
Steps to Install
Clone this repository:
bash
Copy code
git clone https://github.com/your-repo/ipa-feature-lookup.git
Navigate to the project directory:
bash
Copy code
cd ipa-feature-lookup
Install required libraries:
bash
Copy code
pip install -r requirements.txt
Run the app:
bash
Copy code
python ipa_lookup.py
Dataset
The app uses a preloaded dataset containing IPA symbols and their phonological features. You can extend or customize the dataset by editing the ipa_features dictionary or uploading a JSON/CSV file.

Example Dataset Format
python
Copy code
ipa_features = {
    "b": {
        "consonantal": "+",
        "sonorant": "-",
        "voice": "+",
        "nasal": "-",
        "labial": "+",
        "dorsal": "-",
        "coronal": "-"
    },
    "p": {
        "consonantal": "+",
        "sonorant": "-",
        "voice": "-",
        "nasal": "-",
        "labial": "+",
        "dorsal": "-",
        "coronal": "-"
    }
}
Future Enhancements
Batch Lookup: Support for multiple IPA phones at once.
Web-Based Interface: A web version using Flask or Django.
Export Features: Save results to a CSV or text file.
Interactive Visualizations: Add graphical representation of feature distributions.
Contributing
We welcome contributions to improve this tool! If you’d like to contribute:

Fork the repository.
Create a feature branch.
Submit a pull request with your changes.
