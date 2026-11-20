# AI Shopping Agent

Chat to search a grocery catalog ("find me organic honey under $20 with 4.5+ rating") and place orders. Built with LangChain, Streamlit, and `openai/gpt-oss-120b` on GroqCloud.

Hosted in Streamlit url: https://ai-grocery-shopping-agent-2gdlqcmdqhkugmgfc4mbsb.streamlit.app/

## Run

1. Copy `.env.example` to `.env` and add your `GROQ_API_KEY`.
2. `uv sync`
3. `uv run streamlit run app.py`

The SQLite database (`resources/store.db`) is created automatically on first run, or manually with `uv run python -m src.setup_db`. Orders are inserted into the `orders` table.
<img width="1920" height="1080" alt="Screenshot from 2026-11-20 12-11-18" src="https://github.com/user-attachments/assets/587f937e-41a7-469c-82eb-a13fb025638a" />

