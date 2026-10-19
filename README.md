# 📄 Document Q&A

A small Streamlit app that lets you upload a document and ask questions about it. It sends your file and question to OpenAI and streams the answer back, so you can pull out a summary or a specific detail without reading the whole thing yourself.

I built it to make getting through long notes and docs a bit quicker.

## Getting Started

You'll need Python 3.8+ and an [OpenAI API key](https://platform.openai.com/account/api-keys).

1. Install the dependencies:

   ```
   pip install streamlit openai
   ```

2. Run the app:

   ```
   streamlit run streamlit_app.py
   ```

3. Enter your API key, upload a `.txt` or `.md` file, and ask your question.

## Tips

- Questions like "Give me a short summary" or "What are the action items?" work well.
- To avoid pasting your key every time, store it in `.streamlit/secrets.toml` and load it with `st.secrets`.
- The model is set in the code (`gpt-3.5-turbo` by default), so you can swap in a different one if you like.
