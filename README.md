An AI-powered chatbot that allows users to interact with YouTube videos by asking questions about their content. 
The application extracts the video's transcript, splits it into meaningful chunks, converts the chunks into vector
embeddings using Google Gemini Embeddings, and stores them in a FAISS vector database

When a user asks a question, the system retrieves the most relevant transcript chunks and provides them as
context to a Gemini LLM, which generates a relevant and context-aware response. 
This project demonstrates the practical implementation of a Retrieval-Augmented Generation (RAG) pipeline.
Key Features-
Extracts transcripts from YouTube videos
Supports Hindi/English transcripts when available
Splits long transcripts into manageable chunks
Generates semantic embeddings using Gemini
Stores and searches embeddings using FAISS
Retrieves relevant context for user queries
Generates context-aware answers using Gemini
Implements a complete Retrieval-Augmented Generation (RAG) workflow

Tech Stack
Python
LangChain
Google Gemini API
Gemini Embeddings
FAISS
YouTube Transcript API
RAG (Retrieval-Augmented Generation)

Project Workflow-
Indexing – Extract the transcript from the YouTube video.
Text Splitting – Divide the transcript into smaller overlapping chunks.
Embedding – Convert each chunk into a numerical vector using Gemini Embeddings.
Vector Storage – Store the vectors in FAISS for efficient similarity search.
Retrieval – Retrieve the most relevant chunks based on the user's query.
Generation – Pass the retrieved context and query to Gemini to generate the final response.
