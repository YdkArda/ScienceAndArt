# 🚀 AI Model Inference Application (Streamlit & Hugging Face)
This Jupyter/Colab notebook allows you to quickly run a Streamlit application capable of performing both Text-to-Text and Text-to-Image tasks.

The application is configured to run on a GPU (T4 recommended) in Google Colab.
## 🛠️ How It Works

Bu defterde aşağıdaki iki temel AI işlevi sunulmaktadır:

| Mod | Kullanılan Model | Amaç |
| :--- | :--- | :--- |
| **Text to Text(LLM)** | **Mistral 7B Instruct v0.2** (8-bit Nicemleme) | Generates responses to text prompts with advanced generation settings (Top-P, Repetition Penalty). |
| **Text to Image** | **FLUX.1-dev** (Hugging Face Inference API) | TGenerates high-resolution (1024x1024) images using Text-to-Image prompts. |

## 📦 Setup and Running Steps
Running the application involves just 3 simple steps:

Step 1: Install Dependencies

### STEP 1: INSTALL DEPENDICIES

Run the first code cell. This step installs necessary Python libraries like Streamlit, bitsandbytes, accelerate, and pyngrok.


### STEP 2 : CREATING SECRETS
The next cell creates a file in Colab so Streamlit can access the secrets.

### STEP 3: ADDING HUGGING FACE TOKEN

This code block allows you to save your Hugging Face token to the file. 

Note: You need to paste your own Hugging Face token here.
### STEP 4: CHECK
 This code block shows that the correct data has been saved to the secrets. When run, your Hugging Face token in the format hf-**** should be displayed.
### STEP 5 RUN
The main code block: -- Contains the Streamlit code; every statement written in the code is processed into the app.py file. The block needs to be run for the changes to be written.

The final block creates the development server via ngrok. The Streamlit application can be viewed via the link generated when the code runs.
