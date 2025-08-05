# Project Summary:-
This is a GenAI-powered document QA system that takes a PDF report (like a TCS financial report), splits it into manageable chunks, 
generates semantic embeddings, stores them in a FAISS vector database, and allows intelligent querying using OpenAI's GPT model.

1. PDF Loading :- Loads a full PDF document using LangChain's PyPDFLoader.

2. Text Splitting :- Splits the long document into small overlapping chunks. Helps preserve context for better understanding.

3. Embeddings Creation :- Uses a lightweight, fast HuggingFace sentence transformer to convert text into vectors.

4. FAISS Vector Store :- Stores the chunked, embedded data into a FAISS vector index for fast similarity search.

5. Semantic Search :- Performs similarity search to fetch top relevant chunks for a given user query.

6. Contextual Prompt to GPT :- Combines the retrieved context with the question in a prompt that is passed to GPT.
 
7. Generating Answer :- Uses GPT-4o-mini to generate accurate, grounded responses strictly based on the context.

# Use Case:-
You can use this setup to ask specific, factual questions about lengthy PDF documents — like financial reports, contracts, legal papers, or whitepapers.


   
   
