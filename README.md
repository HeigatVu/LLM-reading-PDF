# Retrieval Augmented Generation (RAG) for PDF - Question Answering project on AIO2024 Course

[![License: AI VIETNAM](https://scontent.fsgn19-1.fna.fbcdn.net/v/t39.30808-6/326762542_533351005436945_3355631653176967012_n.png?_nc_cat=105&ccb=1-7&_nc_sid=6ee11a&_nc_eui2=AeE9pOsTEb7zxmRQrvyUBPxgtF52D5hLN4O0XnYPmEs3g7AlMLgEk3fAp7aFuzj6N7_pHZY75KuK2hkn9QFlKhTI&_nc_ohc=RKGdWrggtYQQ7kNvgHyNqOv&_nc_ht=scontent.fsgn19-1.fna&cb_e2o_trans=t&oh=00_AYDul-l8EEwNeIkfQn3WcrS_EnX0GgO6pVPbDRwM9LKR2Q&oe=668F3B3F)](https://www.facebook.com/aivietnam.edu.vn)

This project demonstrates how to build a Retrieval Augmented Generation (RAG) system for question answering on educational materials, specifically targeting the AI Việt Nam (AIO) course content.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
- [Usage](#usage)
- [Example](#example)
- [Key Concepts](#key-concepts)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Large Language Models (LLMs) like ChatGPT are powerful but can benefit from external knowledge sources. RAG combines LLMs with information retrieval to provide more accurate and contextually relevant answers. This project showcases how to apply RAG to educational PDFs, making course materials more interactive and accessible.

## Features

- **PDF Question Answering:** Ask questions about your AIO course materials in natural language.
- **Retrieval-Augmented Responses:**  The system retrieves relevant passages from the PDF to enhance the accuracy of the LLM's answers.
- **Interactive Chat Interface (Optional):** Engage in a conversation with your course materials using a user-friendly chat interface.

## Getting Started

### Prerequisites

- Python 3.x
- GPU access (recommended for running the Vicuna LLM)
- Required libraries (install via `pip install -r requirements.txt`)

### Installation

1. Clone this repository: `git clone https://github.com/NiranVu/LLM-reading-PDF.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Download the AIO course material PDF and place it in the project directory.

## Usage

1. **Basic RAG:**
   - Run the `rag.py` script.
   - Enter your question when prompted.
   - The system will output the answer along with relevant source passages.

2. **Interactive Chat Interface (Optional):**
   - Run the `app.py` script using Chainlit: `chainlit run app.py`
   - Follow the instructions to upload your PDF and start chatting.

## Example
**I gave this model a PDF about YOLOv10 and I asked about this PDF**
- **Question**: YOLOv10 là cái gì?
- **Answer**: YOLOv10 là một phiên bản của YOLO (You Only Look Once) - một hệ thống dự đoán mẫu được sử dụng để tìm kiếm các mẫu được trong các ảnh. Nó được sử dụng cho việc dự đoán các mẫu trong các ảnh với tốc độ nhanh và chính xác. Trong bài viết này, nhóm cung cấp các bước cài đặt và sử dụng YOLOv10 để dự đoán các mẫu trong các ảnh.

## Key Concepts

- **LangChain:** A framework for developing LLM-powered applications.
- **Chroma:** A vector database for storing and retrieving document embeddings.
- **Hugging Face Transformers:** A library for working with pre-trained language models like Vicuna.
- **Chainlit:** A library for building chat interfaces for LLM applications.
