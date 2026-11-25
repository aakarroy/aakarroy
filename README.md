<div align="center">

<h1>Aakar Roy</h1>

**AI/ML engineering student building applied systems in computer vision, medical imaging, and LLMs.**

Currently building SamDrishti, an assistive technology project for visually impaired users.

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![MONAI](https://img.shields.io/badge/MONAI-0D9488?style=for-the-badge)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-0B7285?style=for-the-badge)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6446?style=for-the-badge)
![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-3E7CB1?style=for-the-badge)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)

[LinkedIn](https://www.linkedin.com/in/aakar-roy-a689aa333) &nbsp;|&nbsp; [Email](mailto:iamaakarroy@gmail.com) &nbsp;|&nbsp; [Project Portfolio](https://my-projects-aakar-roy.streamlit.app/)

 [Projects](#projects) &nbsp;|&nbsp; [Selected Work](#selected-work)

</div>


## Projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/aakarroy/vashist.ai">Vashist AI</a></h4>
      <p>Fully local, privacy-first RAG study assistant over PDFs, slides, and web URLs.</p>
      <p><b>Problem:</b> cloud study assistants require uploading personal study material to third-party servers.</p>
      <p><b>Approach:</b> an end-to-end local pipeline with document and image ingestion, ChromaDB retrieval, Qwen2.5:3b via Ollama, and PII masking on both input and output.</p>
      <p><code>Python</code> <code>RAG</code> <code>Ollama</code> <code>ChromaDB</code></p>
    </td>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/aakarroy/ToothFairy2">ToothFairy2</a></h4>
      <p>End-to-end 3D multi-class tooth segmentation on dental CT/CBCT using MONAI and a 3D Residual U-Net.</p>
      <p><b>Problem:</b> delineating individual teeth in volumetric dental scans is slow to do by hand.</p>
      <p><b>Approach:</b> a 3D Residual U-Net trained with MONAI to segment teeth by class, with a separate jaw-separation output.</p>
      <p><code>PyTorch</code> <code>MONAI</code> <code>3D Segmentation</code></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/TridibeshSam31/Retail-Store-Agent">Ware Agent</a></h4>
      <p>Multi-agent system where per-store agents and an arbitrator negotiate inventory rebalancing from ML demand forecasts.</p>
      <p><b>Problem:</b> manual, gut-feel stock reordering across a retail chain.</p>
      <p><b>Approach:</b> an ML demand forecaster, one agent per store, and a neutral arbitrator that detect shortages, locate surplus elsewhere, and propose a resolution automatically.</p>
      <p><i>Team project. My role: designing and implementing the agentic workflow.</i></p>
      <p><code>Python</code> <code>LangGraph</code> <code>Forecasting</code></p>
      <p><a href="https://retail-store-agent.vercel.app/">Live Demo</a></p>
    </td>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/aakarroy/Open-Vision">Aerial Turf Segmentation (Open Vision)</a></h4>
      <p>Binary semantic segmentation of turf in aerial imagery with U-Net and YOLOv8, producing GIS-ready outputs.</p>
      <p><b>Problem:</b> turf regions in high-resolution aerial imagery need to be identified in a form GIS workflows can use.</p>
      <p><b>Approach:</b> U-Net and YOLOv8 architectures for segmentation, with inference outputs designed to be GIS-native.</p>
      <p><code>PyTorch</code> <code>U-Net</code> <code>YOLOv8</code></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/aakarroy/Pneumonia-Detection">Pneumonia Detection</a></h4>
      <p>Chest X-ray classification with a custom CNN, deployed as a real-time Streamlit app.</p>
      <p><b>Problem:</b> a fast first-pass screening aid for chest X-rays.</p>
      <p><b>Approach:</b> a custom CNN in PyTorch, served through a Streamlit interface for real-time prediction, with evaluation metrics shown below.</p>
      <p><code>PyTorch</code> <code>CNN</code> <code>Streamlit</code></p>
    </td>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/aakarroy/Machine-Learning-Algorithms">Machine Learning Algorithms</a></h4>
      <p>Linear, logistic, and polynomial regression applied to housing, cardiac risk, and manufacturing datasets.</p>
      <p><b>Problem:</b> building a solid grounding in core algorithms before moving to deep learning.</p>
      <p><b>Approach:</b> each algorithm applied end to end to a real dataset, including a StandardScaler and PolynomialFeatures pipeline for the polynomial model.</p>
      <p><code>scikit-learn</code> <code>Pandas</code> <code>Seaborn</code></p>
    </td>
  </tr>
</table>

## Selected Work

### Vashist AI: system architecture

A local retrieval pipeline with security and caching built in. Every stage runs on the user's machine.

```mermaid
%%{init: {"theme":"base","themeVariables":{"fontSize":"11px","lineColor":"#2A9D8F"},"flowchart":{"nodeSpacing":20,"rankSpacing":24,"padding":10,"htmlLabels":true}}}%%
flowchart LR
    subgraph ING["Ingestion"]
        direction TB
        A["PDF / PPTX / URL"] --> B["Loaders<br/>PyMuPDF, UnstructuredPPT,<br/>Jina Reader<br/>Image Extraction"]
        B --> C["Text chunking<br/>Qwen 2.5 Tokenizer<br/>1000-token chunks"]
        B --> D["Image captioning<br/>microsoft/git-base<br/>HuggingFace"]
        C --> E["Embeddings<br/>nomic-embed-text<br/>via Ollama"]
        D --> E
        E --> F[("ChromaDB<br/>Cosine Similarity<br/>Persistent on Disk<br/>Unified Text + Image Captions")]
    end

    subgraph QRY["Query"]
        direction TB
        Q["User Query<br/>Qwen2.5:3b<br/>Multi-query expansion<br/>+2 query variants"] --> R["Retriever<br/>Query Embedding<br/>Top-K + Score Filter<br/>Text Chunks + Image Captions"]
        R --> PI["PII Input Detection<br/>Regex Scan + Masking"]
        PI --> CA["Cache Lookup<br/>CacheLayer<br/>SHA-256 Key + TTL<br/>In-memory"]
        CA --> G["Generation<br/>Qwen2.5:3b via Ollama<br/>Meta-Prompt: Expert Role<br/>Context-grounded Answer<br/>LLM Knowledge Fallback"]
        G --> OV["Output Validation<br/>PII Masking<br/>Harmful Content Check"]
        OV --> OUT["Final Answer<br/>Source References<br/>Visual Asset Paths"]
    end

    ING -.->|"vector store"| QRY

    classDef n fill:#E6F4F1,stroke:#2A9D8F,stroke-width:1.5px,color:#1F2933
    class A,B,C,D,E,F,Q,R,PI,CA,G,OV,OUT n

    style ING fill:#F6F8FA,stroke:#2A9D8F,color:#1F2933
    style QRY fill:#F6F8FA,stroke:#2A9D8F,color:#1F2933
```

### ToothFairy2: 3D segmentation output

<div align="center">
  <table>
    <tr>
      <td width="50%" align="center">
        <img src="assets/023_FDI.gif" alt="Tooth segmentation" width="100%">
        <br><sub>Multi-class tooth segmentation (FDI labels)</sub>
      </td>
      <td width="50%" align="center">
        <img src="assets/023_Jaw-Separation.gif" alt="Jaw segmentation" width="100%">
        <br><sub>Upper and lower jaw separation</sub>
      </td>
    </tr>
  </table>
</div>

### Pneumonia Detection: metrics and predictions

<table>
  <tr>
    <td width="50%" align="center">
      <img src="assets/Predictions-Metrics.png" alt="Pneumonia Detection metrics" width="100%">
      <br><sub>Prediction metrics</sub>
    </td>
    <td width="50%" align="center">
      <img src="assets/Prediction.png" alt="Pneumonia Detection sample prediction" width="100%">
      <br><sub>Sample prediction on test data</sub>
    </td>
  </tr>
</table>

### Open Vision: aerial turf segmentation

<table>
  <tr>
    <td width="50%" align="center">
      <img src="assets/1785406913079.jpg" alt="Aerial segmentation result 1" width="100%">
      <br><sub>Test result 1</sub>
    </td>
    <td width="50%" align="center">
      <img src="assets/1785406913162.jpg" alt="Aerial segmentation result 2" width="100%">
      <br><sub>Test result 2</sub>
    </td>
  </tr>
</table>
