# Offline_ChatGpt_like_app

**Future Development:**
I plan to enhance this project by implementing it to work with proprietary user data rather than public data. This upgrade will involve training the system on custom datasets and deploying it offline to ensure data security and privacy. The goal is to provide a tailored, secure, and contextually accurate question-answering solution for specific organizational needs.

**Project Overview:**
I have developed a question-answering PDF chatbot utilizing a combination of LangChain, OpenAI, Panel, and Hugging Face technologies. This chatbot allows users to upload PDF files, ask questions, and receive answers based on the contents of the uploaded document. The application features an interactive dashboard and supports various querying methods.

**Technologies Used:**
1. **LangChain**: A framework for building language model applications.
2. **OpenAI**: Provides the language model API for generating answers.
3. **Panel**: Used for creating the interactive dashboard interface.
4. **Hugging Face**: Hosts alternative language models and tools for additional integration options.

**Achievements:**

1. **Application Setup and User Interface:**
   - **Panel Integration**: I created an interactive web interface using Panel, which includes:
     - **File Input Widget**: Users can upload PDF files.
     - **Question Input Widget**: A text field for users to enter their questions.
     - **Run Button**: Executes the query against the uploaded document.
     - **Advanced Settings**: Options to select the chain type (e.g., Inline, MapReduce) and specify the number of text chunks to process.

2. **Question Answering Functionality:**
   - **PDF Processing**: I utilized `PiPDFLoader` from LangChain to load and preprocess PDF documents.
   - **Document Chunking**: Split documents into manageable chunks for efficient querying.
   - **Retrieval QA Chain**: Implemented a retrieval-based question-answering system using LangChain, which:
     - Creates Vector stores to index and retrieve text chunks.
     - Performs similarity searches to find relevant text chunks for answering queries.
     - Uses OpenAI’s API to generate answers based on retrieved text chunks.

3. **OpenAI Integration:**
   - **API Integration**: Integrated OpenAI’s API to generate responses based on queries and relevant text chunks extracted from the PDF.
   - **API Key Management**: Ensured secure handling of the OpenAI API key through a password input widget.

4. **Hugging Face Integration:**
   - **Alternative Models**: Provided the option to use models from Hugging Face as alternatives to OpenAI’s API, allowing users to select from various language models available on the Hugging Face platform.

5. **User Interaction and Results Display:**
   - **Interactive Dashboard**: Developed an engaging user interface using Panel to display:
     - Details of the uploaded PDF file.
     - User questions and corresponding answers.
     - Relevant source text chunks from the PDF.
   - **Chat History**: Maintained a history of questions and answers, displaying them sequentially in the interface.

6. **Deployment and Hosting:**
   - **Local Deployment**: Configured the application for local deployment using a Docker container, including:
     - **Dockerfile**: Defined environment setup, package installations, and application serving.
     - **Permissions Management**: Handled file permissions for storing and reading PDFs.

**Summary:**
This project successfully integrates LangChain, OpenAI, Panel, and Hugging Face technologies to create a robust question-answering chatbot capable of processing and answering queries based on PDF documents. The application features a user-friendly interface, advanced settings for customization, and support for alternative language models. Moving forward, I will focus on implementing this solution with proprietary user data and enhancing its capabilities for offline deployment and improved data security.
