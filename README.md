# End-to-end-medical-chatbot-using-Lama2

# How to run?
### STEPS:

Clone the repository

```bash
Project repo: https://github.com/
```

### STEP 01- Create a conda environment after opening the repository

```bash
conda create -n mchatbot python=3.8 -y
```

```bash
conda activate mchatbot
```

### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```


### Create a `.env` file in the root directory and add your FAISS vector database credentials as follows:

```ini
FAISS_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```


### Download the quantize model mentioned below & keep the model in the model directory:

```ini
## Download the Llama 2 Model:

llama-2-7b-chat.ggmlv3.q4_0.bin


## From the following link:
https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/tree/main
```

```bash
# run the following command
python store_index.py
```

```bash
# Finally run the following command to run the project on Flask server
python app.py
```

Now,
```bash
Open up http://localhost:5000 in your browser to interact with the Medical Chatbot.
```


### Techstack Used:

- Python
- LangChain
- Flask
- Meta Llama2
- FIASS


