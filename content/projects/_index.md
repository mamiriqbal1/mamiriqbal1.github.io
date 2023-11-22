---
title: "Projects"
draft: false
---

Following is a list of some of my personal projects:

## Implementing retrieval augmented generation (RAG) for a book

I have create a notebook that demonstrate how you can implement retrieval
augmented generation for a book. I have used the O Level computer science book
for this purpose. You can use it with any of your favorite large language models
(LLM) for example chatgpt or llama2.

### 🚀 How retrieval augmented generation works

Following are the high level steps needed for the implementation for retrieval
augmented generation.

1. Extract text from source. If the source is unstructured, like PDF, the
   extraction can be a challenge.
2. Index the extracted text, often as vector embeddings and store.
3. Let the user ask questions related to the source.
4. Perform a similarity search in the index and retrieve relevant text chunks.
5. Insert these text chunks in the prompt along with the question.
6. Request an LLM (e.g. chatgpt) to produce an answer _only_ based on the
   context

### 🧨 Name of the game

The success of any RAG implementation mainly depends on the following aspects

1. The quality of input data. If the data is unstructured, you need to carefully
   analyze and extract relevant and useful text only. The quality of input
   determines the quality of the answers you will get from LLM.
2. You should to experiment with chunk sizes and overlaps that are suitable for
   your application
3. You should test different number of top similar results that gives the best
   performance.
4. You can not have a universal prompt template that will work with every LLM.
   You will have to fine-tune the prompt for the specific LLM you are using in
   order to get best results.

[github](https://github.com/mamiriqbal1/rag_book_qa_prompt)

## Image Classification using Learning Classifier Systems

I created an image classifier (XCS-IMG) using evolutionary machine learning.
XCS-IMG is the adaptation of accuracy based learning classifier system (XCS) for
images. It is a step towards explainable artificial intelligence (XAI). I have
demonstrated how the evolved rules can be visualized to explain the
classification result. The system uses concept of filters that are evolved
during the learning phase to capture image features that can be visualized.

[github](https://github.com/mamiriqbal1/XCS-IMG)

## Scraping Dynamic Websites using Puppeteer

I have created a small project based on Puppeteer that can scrape a website with
continuous scrolling. Puppeteer uses a headless browser to successfully
javascript rendered websites.

[github](https://github.com/mamiriqbal1/continuous-scroll-scraping)
