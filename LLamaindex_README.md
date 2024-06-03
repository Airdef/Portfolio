### Description
The model is configured to answer questions based on the specific knowledge space of the uploaded PDF. However, users can modify the code to enable the model to generalize responses, allowing it to correctly answer questions in contexts different from the original knowledge space. This generalization can be achieved using techniques such as deploying multiple agents or crafting custom prompts.

- model: gpt-3.5-turbo
- embeddings: text-embedding-3-small
- Python version: 3.10.12
  
### Requirements
- Google Chrome: Recommended for accessing Google Colab, as it provides the most stable and consistent experience, particularly for file uploads and session management.
  Note: While other browsers might work, Google Chrome is preferred to avoid potential issues with file handling and interface compatibility.
- Google Colab: The code is intended to be executed in a Google Colab environment.
- OpenAI API Key: You will need an API key from OpenAI to interact with their models.
- PDF Document: A PDF file that serves as the knowledge base for the application.

### Getting Started

## Direct Link from GitHub :

You can  access the notebook directly from GitHub thanks to the embedded Colab link in the .ipynb file. 
  
## Run  Code on Colab
- Execute a Cell: Click on a cell with code and press the play button on the left of the cel.
- Run All Cells: To execute all the cells in the notebook, go to Runtime > Run all.
  
## Configuring Your OpenAI API Key

- Obtain an API key from [OpenAI](https://openai.com/):
  - Sign up or log in to your OpenAI account.
  - Navigate to the API section and generate a new API key.

- Once you have your API key, enter it when prompted by the notebook in Google Colab. This key is used to authenticate your requests to the OpenAI API.

## Uploading Your PDF Knowledge Base

- When the Colab notebook prompts you to upload a PDF, use the file upload feature in Colab to select and upload your PDF document from your local machine to the specified directory.

0. Wait Colab notebook to prompt you to upload a PDF

1. Open the Files Sidebar: On the left side of your Colab notebook, click on the folder icon to open the "Files" sidebar.

2. Refresh the File List (if the specified directory (`KW_space`)): At the top of the Files sidebar, there is a refresh icon. Click this icon to refresh the directory listing. 

3. Navigate to the Directory: when the code ask to upload the PDF, navigate into the specified directory (`KW_space`) within the Files sidebar.

4. Upload Files: Right-click within the Files sidebar (inside the specified directory: `KW_space` ) and select "Upload". Choose the PDF file from your local machine that you want to upload.

5. Verify Upload: After the upload completes, you should see the file listed in the Files sidebar under the specified directory (`KW_space`).

## Usage

Please follow the instructions within the notebook to:
- Input your OpenAI API key
- Input the PDF (i.e: PDF TEST FILE)
- Ask question to the llm
- Insert `exit` in the Question space to terminate the cell
