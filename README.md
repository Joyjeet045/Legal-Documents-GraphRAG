# Legal IT Law Q&A System: Knowledge Graphs & LLMs

A sophisticated question-answering system that demonstrates the power of combining **Knowledge Graphs**, **Retrieval-Augmented Generation (RAG)**, and **Large Language Models (LLMs)** for legal document analysis and retrieval. This system was built using **Indonesian IT Law** as a comprehensive example to showcase how modern AI techniques can make complex legal frameworks more accessible and navigable.

<br>

## Overview
Indonesia's IT legal framework comprises a vast number of regulations, articles, and interconnections, making it complex to navigate. This system leverages **Retrieval-Augmented Generation (RAG)**, **Large Language Models (LLMs)**, and **Knowledge Graphs** to deliver a smarter, context-aware **Q&A platform** that enables legal professionals, researchers, and policymakers to retrieve precise legal insights efficiently.

## Features
This system allows users to:
- Perform **AQL (ArangoDB Query Language)** and **semantic searches** across 63 Indonesia IT law regulations.
- Identify **the most influential regulations** and explore their relationships.
- Analyze **connections between regulations and articles** using graph-based analytics.
- Visualize legal structures with **matplotlib** for better understanding.

## Installation
To install the latest version of this code, please use this following command.
1. Git clone this project to the local computer
    ```shell
    git clone https://github.com/bayu-siddhi/graph-rag-arangodb
    cd graph-rag-arangodb
    ```

2. Create a virtual environment (optional but recommended):.
    ```shell
    python -m venv venv
    source venv/bin/activate  # on Windows: venv\Scripts\activate
    ```

3. Install all the project dependencies.
    ```shell
    pip install -r requirements.txt
    ```

4. Copy the environment configuration.
    ```shell
    cp .env.example .env
    ```

5. Run the Gradio app on the [`main.py`](main.py) file.
    ```shell
    python main.py
    ```
    Or see the development process in [`notebook.ipynb`](notebook.ipynb).

> [!NOTE]
> - This project was developed using `python==3.11.4`, see [requirements.txt](requirements.txt) for dependencies details.
> - Edit the `.env` file and fill in your ArangoDB credentials and other necessary configuration.
> - Make sure ArangoDB is running and that the user has Administrate privileges.

## Technical Architecture  
1. **Knowledge Graph Construction:**  
   - **ArangoDB** serves as the graph database foundation, storing **63 regulations**, **2,423 articles**, and over **7,500 relationships** including amendments, references, and hierarchical structures.
2. **Graph Analytics:**
   - **NetworkX** integration enables analysis of **shortest paths, centrality metrics, and community structures**.
3. **Natural Language Processing:**
   - **RAG with LLMs** provides **context-aware responses** based on intelligent graph retrieval.
4. **User Interface:**
   - **Gradio** framework powers the interactive interface, running locally at `http://127.0.0.1:7861`.

## Technical Challenges
- Efficiently indexing and querying **large-scale legal documents** while maintaining response speed.
- Integrating **graph-based retrieval** with **LLM-generated** responses.
- Designing an intuitive **legal Q&A interface** for non-technical users.

## Key Achievements
- **Seamless integration** of ArangoDB, NetworkX, and LLMs delivering **graph-enhanced legal Q&A** capabilities.
- **Advanced legal reasoning** through comprehensive mapping of **impact and cross-references** between regulations.
- **Interactive visualization system** that dynamically displays legal connections and relationships.

## Key Discoveries & Learnings
- **RAG and LLMs** demonstrate exceptional effectiveness in **legal document retrieval** and analysis.
- **Knowledge graphs significantly enhance Q&A accuracy** by transforming unstructured legal data into structured, queryable formats.
- **Graph analytics prove essential in legal research**, particularly for identifying key regulatory influences and dependencies.
