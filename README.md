# Chat Application with Retrieval-Augmented Generation (RAG)

This repository contains a chat application implemented in a Jupyter Notebook, utilizing Retrieval-Augmented Generation (RAG) with Gemini model. The application uses Pinecone to fetch relevant context from a predefined conversation history.

## Features

- Retrieval of relevant historical messages using Pinecone
- Integration with Gemini model to generate responses
- Token limit management using the Hugging Face `transformers` library
- Easy setup and deployment

## Prerequisites

- Python 3.7 or higher
- Jupyter Notebook
- Pinecone API Key
- Gemini API Key

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/chat-rag-app.git
    cd chat-rag-app
    ```

2. Install the required Python packages:

    ```bash
    pip install pinecone-client
    pip install protoc_gen_openapiv2
    pip install -q -U google-generativeai
    pip install tiktoken
    ```

## Usage

### Step 1: Initialize Pinecone and OpenAI

In the first cell of your Jupyter Notebook, initialize Pinecone and OpenAI. Refer to the initialization code for details.

Step 2: Define Functions

Define the necessary functions to generate embeddings, add embeddings to Pinecone, retrieve relevant history, prepare the prompt, and test the final prompt. Refer to the following files for each function:

	•	generate_embedding
	•	add_embeddings_to_pinecone
	•	retrieve_relevant_history
	•	prepare_prompt
	•	test_final_prompt

Step 3: Add Conversation History to Pinecone

Add the predefined conversation history to Pinecone. Refer to the conversation history code for details.

Step 4: Run the Test

Run the test_final_prompt function to generate a response using the prepared prompt. Refer to the test_final_prompt code for details.
