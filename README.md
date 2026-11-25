<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/banner-light.svg">
  <img alt="Aakar Roy - AI/ML Engineering" src="assets/banner-light.svg" width="100%">
</picture>

<p align="center">
  <a href="#projects">Projects</a> &nbsp;|&nbsp;
  <a href="#selected-work">Selected Work</a> &nbsp;|&nbsp;
  <a href="#technical-stack">Stack</a> &nbsp;|&nbsp;
  <a href="#contact">Contact</a>
</p>

---

## About

AI/ML engineering student building applied machine learning systems across computer vision, medical imaging, and LLM-based applications. Currently building SamDrishti, an assistive technology project for visually impaired users.

---

## Projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/aakarroy/vashist.ai">Vashist AI</a></h4>
      <p>Fully local, privacy-first RAG study assistant over PDFs, slides, and web URLs.</p>
      <p><code>Python</code> <code>RAG</code> <code>Ollama</code> <code>ChromaDB</code></p>
    </td>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/aakarroy/ToothFairy2">ToothFairy2</a></h4>
      <p>End-to-end 3D multi-class tooth segmentation on dental CT/CBCT using MONAI and a 3D Residual U-Net.</p>
      <p><code>PyTorch</code> <code>MONAI</code> <code>3D Segmentation</code></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/TridibeshSam31/Retail-Store-Agent">Ware Agent</a></h4>
      <p>Multi-agent system where per-store agents and an arbitrator negotiate inventory rebalancing from ML demand forecasts.</p>
      <p><code>Python</code> <code>LangGraph</code> <code>Forecasting</code></p>
    </td>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/aakarroy/Open-Vision">Aerial Turf Segmentation</a></h4>
      <p>Binary semantic segmentation of turf in aerial imagery with U-Net and YOLOv8, producing GIS-ready outputs.</p>
      <p><code>PyTorch</code> <code>U-Net</code> <code>YOLOv8</code></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/aakarroy/Pneumonia-Detection">Pneumonia Detection</a></h4>
      <p>Chest X-ray classification with a custom CNN, deployed as a real-time Streamlit app.</p>
      <p><code>PyTorch</code> <code>CNN</code> <code>Streamlit</code></p>
    </td>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/aakarroy/Machine-Learning-Algorithms">Machine Learning Algorithms</a></h4>
      <p>Linear, logistic, and polynomial regression applied to housing, cardiac risk, and manufacturing datasets.</p>
      <p><code>scikit-learn</code> <code>Pandas</code> <code>Seaborn</code></p>
    </td>
  </tr>
</table>

---

## Selected Work

### Vashist AI: system architecture

```mermaid
flowchart TD
    classDef node fill:#0F2A35,stroke:#2A9D8F,color:#E6F1F5,stroke-width:1.5px
    classDef store fill:#12343F,stroke:#2A9D8F,color:#E6F1F5,stroke-width:2px

    subgraph Ingestion
        A["Data Sources<br/>PDF / PPTX / URL"] --> B["Document Loaders<br/>PyMuPDF / UnstructuredPPT / Jina Reader<br/>+ image extraction"]
        B -->|Text| C["Chunking<br/>Qwen2.5 tokenizer, 1000-token chunks"]
        B -->|Images| D["Captioning<br/>microsoft/git-base"]
        C --> E["Embeddings<br/>nomic-embed-text via Ollama"]
        D --> E
        E --> F[("ChromaDB<br/>Persistent, cosine space<br/>Unified text + image collection")]
    end

    subgraph Query
        Q["User Query"] --> MQ["Multi-Query Expansion<br/>Qwen2.5:3b, 2 extra variants"]
        MQ --> R["Retriever<br/>Embed, top-K, score filter"]
        R --> PII["Input Security<br/>PII detection and masking"]
        PII --> CA["Cache Lookup<br/>SHA-256 key, TTL, in-memory"]
        CA --> G["Generation<br/>Qwen2.5:3b via Ollama<br/>Meta-prompt role, grounded answer,<br/>fallback to LLM knowledge"]
        G --> OV["Output Security<br/>PII masking, harmful content check"]
        OV --> OUT["Answer + source references<br/>+ visual asset paths"]
    end

    F -.-> R

    class A,B,C,D,E,Q,MQ,R,PII,CA,G,OV,OUT node
    class F store
```

### ToothFairy2: segmentation output

<p align="center">
  <img src="assets/023_FDI.gif" alt="ToothFairy2 3D segmentation demo" width="70%">
</p>

### Pneumonia Detection: prediction results

<p align="center">
  <img src="assets/Predictions-Metrics.png" alt="Pneumonia Detection prediction probabilities" width="60%">
</p>

---

## Technical Stack

| Area | Tools |
|---|---|
| Languages | ![Python](https://img.shields.io/badge/Python-1F2933?style=flat-square&logo=python&logoColor=2A9D8F) ![C++](https://img.shields.io/badge/C++-1F2933?style=flat-square&logo=cplusplus&logoColor=2A9D8F) ![MySQL](https://img.shields.io/badge/MySQL-1F2933?style=flat-square&logo=mysql&logoColor=2A9D8F) |
| Deep Learning | ![PyTorch](https://img.shields.io/badge/PyTorch-1F2933?style=flat-square&logo=pytorch&logoColor=2A9D8F) ![TensorFlow](https://img.shields.io/badge/TensorFlow-1F2933?style=flat-square&logo=tensorflow&logoColor=2A9D8F) ![Keras](https://img.shields.io/badge/Keras-1F2933?style=flat-square&logo=keras&logoColor=2A9D8F) ![MONAI](https://img.shields.io/badge/MONAI-1F2933?style=flat-square) |
| LLM and Agents | ![LangChain](https://img.shields.io/badge/LangChain-1F2933?style=flat-square&logo=langchain&logoColor=2A9D8F) ![LangGraph](https://img.shields.io/badge/LangGraph-1F2933?style=flat-square) ![Ollama](https://img.shields.io/badge/Ollama-1F2933?style=flat-square&logo=ollama&logoColor=2A9D8F) ![ChromaDB](https://img.shields.io/badge/ChromaDB-1F2933?style=flat-square) ![Hugging Face](https://img.shields.io/badge/Hugging_Face-1F2933?style=flat-square&logo=huggingface&logoColor=2A9D8F) |
| ML and Data | ![scikit-learn](https://img.shields.io/badge/scikit--learn-1F2933?style=flat-square&logo=scikitlearn&logoColor=2A9D8F) ![Matplotlib](https://img.shields.io/badge/Matplotlib-1F2933?style=flat-square&logo=matplotlib&logoColor=2A9D8F) ![Seaborn](https://img.shields.io/badge/Seaborn-1F2933?style=flat-square) |
| Deployment | ![Streamlit](https://img.shields.io/badge/Streamlit-1F2933?style=flat-square&logo=streamlit&logoColor=2A9D8F) |

---

## Contact

[LinkedIn](https://www.linkedin.com/in/aakar-roy-a689aa333) | [Email](mailto:iamaakarroy@gmail.com) | [Project Portfolio](https://my-projects-aakar-roy.streamlit.app/)