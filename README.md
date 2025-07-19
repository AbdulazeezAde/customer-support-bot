# Paystack Customer Support Bot

This is a Streamlit-based chatbot for Paystack customer support, leveraging retrieval-augmented generation (RAG) with a local knowledge base and LLMs (OpenAI GPT-3.5-turbo or Gemini-1.5-flash). It uses SentenceTransformer embeddings for semantic search.

## Features
- Summarizes answers in a concise paragraph (no bullet points)
- Uses a local Paystack FAQ/documentation file for context
- Supports both OpenAI and Gemini models (configurable)
- Secure API key management via `.env`
- Modern chat UI with chat history and support info

## Setup
1. **Clone the repository and navigate to the project folder.**
2. **Install dependencies:**
   ```sh
   pip install -r requirements.txt
   ```
3. **Add your API keys to a `.env` file:**
   ```env
   OPENAI_API_KEY=your_openai_key_here
   GEMINI_API_KEY=your_gemini_key_here
   ```
4. **Ensure `Paystack_FAQ_and_Documentation.txt` is in the project directory.**
5. **Run the app:**
   ```sh
   streamlit run chatbot.py
   ```

## Usage
- Select your preferred model in the sidebar.
- Ask questions about Paystack's services, payments, KYC, API, etc.
- The bot will answer using the knowledge base and summarize the answer.

## Notes
- For best results, use a GPU for faster embedding generation (optional).
- The bot will direct users to Paystack support for sensitive or unsupported queries.

## License
MIT License
