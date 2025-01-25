# Vietnamese-RAG-Chatbot
Create a chatbot that provides responses in Vietnamese, focusing on the products offered by a flower shop

Here is the RAG pipeline in two version:
![image](https://github.com/user-attachments/assets/0db9e99f-3a70-463d-a379-f2c41b7e7e31)
![image](https://github.com/user-attachments/assets/c31d8ffc-393b-433b-a709-1d71609b9e6d)

## Prerequisites

- [Python 3.7+](https://www.python.org/downloads/) for running the Streamlit frontend locally
- [pip](https://pip.pypa.io/en/stable/installation/) for managing Python packages
## Clone the repository (or download the code files):

   ```bash
   git clone https://github.com/DucNT17/flower_chatbot.git
   cd flower_chatbot
  ```
## Backend Setup (Flask + Colab + Ngrok)
1. Open the file `rag_flower_chatbot.ipynb` in Kaggle.
2. Make sure to add your `ngrok_key` and `together_api_key`.
3. Run the cell `0.Packages` to install all the dependencies.
4. Run `Data Crawling` to crawl the data if you haven’t done so already.
5. Run `Data Preprocessing` to preprocess the data and perform basic transformations.
6. Run `Retriever Module`, `Answer Generator`, and `Agent Tools` to execute all the components of the RAG pipeline.
7. Run `API` and set the Ngrok URL in the Streamlit files.

## GUI Setup (Streamlit)
1.**Create and activate a virtual environment**

Using venv
```bash
python -m venv venv
venv\Scripts\activate 
```
Using conda
```bash
conda create --name myenv 
conda activate myenv
```
2.**Install dependencies:**
```bash
pip install -r requirements.txt
```
3.**Running the App**

Remember to set the Ngrok URL before running
```bash
streamlit run app.py
```
You can now view your Streamlit app in your browser.

  Local URL: http://localhost:8501
  
  Network URL: http://<your_ip_address>:8501
