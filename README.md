# EXPLAINABLE-AI-FOR-DESTINATION-RECOMMENDER-USING-LLM

This project is a multimodal AI agent that recommends travel destinations based on user **text** input and optional **image** uploads. It combines **BLIP**, **CLIP**, and **LLMs** to analyze preferences and generate human-friendly travel suggestions.

✅ Designed and tested in **Google Colab**  
✅ Compatible with the **GAIA Benchmark** format

This project is designed to run on **Google Colab** and uses the **Hugging Face Inference API** to process input. It also provides a simple **Streamlit interface** for interaction via a localhost tunnel.

---

## 🚀 Features

- Image captioning using **BLIP**
- Tag extraction using **CLIP** + custom logic
- Semantic image search with **FAISS**
- Conversational destination generation via **LLM**
- GAIA-compatible `run_agent(task_input)` interface

---

## 📗 How to Use

### **Download and Open the Colab notebook**

   Make sure you are using **Google Colab** to run this notebook. 
   Download the Main/EXPLAINABLE_AI_FOR_DESTINATION_RECOMMENDER_USING_LLM.ipynb file and upload or open it in [Google Colab](https://colab.research.google.com/).

### **Install required packages (see below)**  

   At the top of the notebook, run the pip install cells.

### **Hugging Face API Token**

We use the **Hugging Face Inference API**, so you need to generate a personal access token:

1. Go to: https://huggingface.co/settings/tokens
2. Click on **New token** → Select **Write** access.
3. Copy the token.

Now in the notebook:
- Search for the keyword `api_key`.
- Replace the placeholder string with your token:
  ```python
  api_key = "[YOUR_HUGGING_FACE_TOKEN]"
  
### **Download and Upload required files**
Download these two files from /Data folder
   1. unsplash_clip.index
   2. unsplash_clip_metadata.csv
      
Click the folder icon on the left sidebar in Colab and upload these two files.

### Run All Cells
Go to the "Runtime" menu → Click "Run all" to execute every cell in sequence.

### Launching the Streamlit App
✅ Step 1:
Run the second-to-last cell – it will generate an IP address. Copy it.

✅ Step 2:
Run the last cell – this will start the Streamlit app and give you a localhost link like:

https://sad-seas-sin.loca.lt

🔐 Paste the IP Address
When you open the link, it will ask for a Tunnel password — paste the IP address you got from the previous cell.

## 📗Demo Video:

https://github.com/user-attachments/assets/058dfa1f-e587-429f-a61b-2518810b774f

