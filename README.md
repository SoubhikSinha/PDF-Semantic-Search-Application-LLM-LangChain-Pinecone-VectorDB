# PDF Semantic Search Application — LLM + LangChain + Pinecone VectorDB

Acknowledgement
---
I would like to extend my sincere thanks to [Krish Naik](https://github.com/krishnaik06) for his invaluable content and guidance, which helped me build this project. This project wouldn't have been possible without his educational resource(s).
<br>
<br>

About the Project
---
This project aimed to explore the practical implementation of [Pinecone](https://www.pinecone.io/) (a cloud-based vector database) and its integration with [LangChain](https://python.langchain.com/docs/introduction/). The goal was to process the content of a PDF document by dividing it into smaller text chunks. These chunks were then converted into vector embeddings using [OpenAI embeddings](https://platform.openai.com/docs/guides/embeddings), which map text data into a high-dimensional vector space. Subsequently, a similarity search (using [cosine similarity](https://www.linkedin.com/pulse/cosine-similarity-large-language-models-llms-ganesh-jagadeesan-zbijc/)) was applied to retrieve relevant answers based on user queries.
<br>
<br>

How to Run this Project ?
---
### **1. Clone the Repository**
Clone the repository to your local machine :
```bash
git clone https://github.com/SoubhikSinha/PDF-Semantic-Search-Application-LLM-LangChain-Pinecone-VectorDB.git
```
<br>

### **2. Create a Virtual Environment**
Navigate to the repository's root directory and create a Conda virtual environment :
```bash
conda create --prefix ./venv python==3.11 -y
```
<br>

### **3. Activate the Conda Environment**
Activate the newly created environment :
```bash
conda activate venv/
```
<br>

### **4. Install Required Libraries**
Install all the necessary dependencies :
```bash
pip install -r requirements.txt
```
<br>


### 5. OpenAI API Secret Key and Pinecone API Key Creation
To access OpenAI models and Pinecone's vector database, follow these steps:

#### **OpenAI API Key Creation🔻**

1.  Navigate to the [OpenAI API Keys webpage](https://platform.openai.com/account/api-keys).
2.  Click on **"Create new secret key"**.
3.  Assign a name to the key for easy identification.
4.  Copy the generated secret key.
5.  Paste the secret key in `.env` file, under the variable name `OPENAI_API_KEY`.

#### **Pinecone API Key Creation🔻**

1.  Visit the [Pinecone API Keys webpage](https://www.pinecone.io/).
2.  Create a new API key for the project.
3.  Copy the generated API key.
4.  Paste the API key in test.ipynb` file in the appropriate section / location.

<br>

### 6. Run the Notebook

To execute the notebook, select the kernel created in the project's root directory (`venv/`) and run all the cells sequentially.
<br>
<br>

### 7. Test with Your Own Query
Feel free to test the implementation using your own query. Ensure that the query is relevant to the content of the selected document to get meaningful results.

