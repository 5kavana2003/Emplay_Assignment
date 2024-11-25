# Emplay_Assignment
This project is designed to extract structured information from various types of documents (PDFs and HTML files) related to the Request for Proposals (RFP) process. The program uses Natural Language Processing (NLP) techniques and Regular Expressions (regex) to extract relevant data from RFP documents and structure it into a predefined format. The structured data is then saved in a JSON file for further use.

Features:
Extracts data from both PDF and HTML documents.
Parses and structures extracted information into predefined fields such as Bid Number, Due Date, Title, and more.
Outputs the structured data in JSON format for easy use and further processing.

Dependencies:
To run this project, you need to install the following Python libraries:
pdfplumber: For extracting text from PDF files.
re: For using regular expressions to identify specific fields in the text.
json: For storing the extracted and structured data in a JSON file.
os: For handling file operations (creating directories, file paths, etc.).

Instructions:
1. Clone the Repository
   Clone this repository or download the project files to your local system.
   git clone <repository_url>

2. Place Your Input Files
   Place your PDF and HTML files in the input/PDFs/ directory. You can include any number of files for processing.

3. Running the Script.
   Once the input files are in place, you can run the Python script. The script will:
   Parse the PDF and HTML files in the input/PDFs/ folder.
   Extract the required fields using regex.
   Structure the extracted data and save it into a JSON file.

4.  Output Files.
    The script will generate a JSON file named structured_data.json in the output directory.
    Optionally, it can also generate a CSV file named structured_data.csv.
    To download the output files from Google Colab, use:
    from google.colab import files
    files.download('output/structured_data.json')

5.   JSON Structure.
     The output JSON file will have the following structure:
     {
  "Bid Number": "JA-12345",
  "Title": "Laptop Purchase",
  "Due Date": "2024-12-31",
  "Bid Submission Type": "Online",
  "Term of Bid": "1 Year",
  "Pre Bid Meeting": "2024-12-01",
  "Installation": "Yes",
  "Bid Bond Requirement": "No",
  "Delivery Date": "2025-01-15",
  "Payment Terms": "Net 30",
  "Any Additional Documentation Required": "No",
  "MFG for Registration": "Dell",
  "Contract or Cooperative to use": "Yes",
  "Model_no": "XYZ-123",
  "Part_no": "12345-67890",
  "Product": "Laptop",
  "contact_info": "contact@company.com",
  "company_name": "Tech Solutions",
  "Bid Summary": "A bid for supplying laptops to schools",
  "Product Specification": "14-inch screen, 8GB RAM, 512GB SSD"
}

 Setup and Prerequisites:
 Ensure that the following steps are completed before running the script:
 1. Python Environment: You should have Python 3.6 or higher installed on your system.
 2. Install Dependencies: Run the pip install command mentioned above to install the required libraries.
 3. Input Files: Place the input PDF and HTML files into the input/PDFs/ folder.

Troubleshooting:
If you encounter any errors related to missing libraries, ensure all dependencies are correctly installed via pip.
Ensure that the input files are properly placed in the specified directory (input/PDFs/).

Conclusion:
This project aims to automate the extraction of structured data from RFP documents, saving time and reducing errors in manual data processing. With the flexibility to handle both PDF and HTML formats, this solution can be adapted for a wide range of document extraction tasks.
