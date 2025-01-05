# Smart Search Tool for Analytics Vidhya Free Courses

This project aims to create an intelligent search tool that helps users efficiently find relevant free courses on the Analytics Vidhya platform. By leveraging a Retrieval-Augmented Generation (RAG) approach, the tool interprets natural language queries or keywords to deliver precise and meaningful results. It is publicly deployed on Huggingface Spaces for evaluation.

# Approach

The tool employs a multi-stage approach:

# Data Collection & Preparation:

Gather course titles, descriptions, and curriculum from Analytics Vidhya's free courses section.
Structure and store this data for efficient processing.
Embedding Generation:

# Divide course data into manageable chunks.
Generate vector embeddings for each chunk using the SentenceTransformer (all-MiniLM-L6-v2) model.
Vector Database & Retrieval:

Store embeddings in Qdrant, a high-performance vector database.
Implement a vector similarity search to retrieve the top 5 most relevant chunks for a given query.
Generative Response Generation:

Utilize a powerful language model (e.g., Google Gemini API or OpenAI GPT-3.5) to process retrieved chunks and generate human-readable responses.
Deployment & User Interface:

Deploy the tool on Huggingface Spaces for easy accessibility.
Create a user-friendly interface using Streamlit for seamless user interaction.
Key Features

Efficient Search: Retrieves highly relevant course information based on user queries.
Concise Responses: Generates clear and informative summaries of relevant courses.
User-Friendly Interface: Provides an intuitive and easy-to-use search experience.
Publicly Accessible: Deployed on Huggingface Spaces for convenient evaluation and usage.
# How It Works

# User Input: The user enters a natural language query or keyword (e.g., "machine learning for beginners").
Search & Retrieval: The system retrieves the most relevant course information chunks from the vector database.
Response Generation: A language model processes the retrieved data and generates a concise and informative response.
Output: The tool presents the user with a list of relevant courses, including brief descriptions and links to the full course details.
Technologies Used

# LangChain: For text chunking and managing the RAG pipeline.
SentenceTransformers: For generating high-quality text embeddings.
Qdrant: For efficient storage and retrieval of embeddings.
Streamlit: For building the user interface.
Google Gemini API or OpenAI GPT-3.5: For generating human-readable responses.
Future Enhancements

# Integrate direct course links for one-click access.
Implement dynamic chunk sizing for improved context capture.
Enhance query understanding with techniques like query expansion.
This project aims to significantly improve the user experience in finding relevant free courses on the Analytics Vidhya platform. The combination of efficient search, high-quality response generation, and a user-friendly interface makes this tool a valuable resource for learners.
