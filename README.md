# EXPLAINABLE-AI-FOR-DESTINATION-RECOMMENDER-USING-LLM

This project is a multimodal AI agent that recommends travel destinations based on user **text** input and optional **image** uploads. It combines **BLIP**, **CLIP**, and **LLMs** to analyze preferences and generate human-friendly travel suggestions.

✅ Designed and tested in **Google Colab**  
✅ Compatible with the **GAIA Benchmark** format

---

## 🚀 Features

- Image captioning using **BLIP**
- Tag extraction using **CLIP** + custom logic
- Semantic image search with **FAISS**
- Conversational destination generation via **LLM**
- GAIA-compatible `run_agent(task_input)` interface

---

## 📗 How to Use

1. **Open the Colab notebook**  
   Upload or open `Copy_of_Merged.ipynb` in [Google Colab](https://colab.research.google.com/).

2. **Install required packages (see below)**  
   At the top of the notebook, run the pip install cells or manually install:

   ```python
   !pip install torch torchvision faiss-cpu transformers sentencepiece \
                 pandas numpy opencv-python Pillow spacy requests tqdm
   !python -m spacy download en_core_web_sm
