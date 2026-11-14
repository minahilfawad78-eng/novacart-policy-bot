# NovaCart Policy Support Bot

Ek chatbot jo sirf NovaCart ki policy files se jawab deta hai. Har jawab mein file aur section ka hawala hota hai. Jo cheez policy mein nahi hoti, usay bot "This is not covered" kehta hai aur andaza nahi lagata.

**Live link:** https://novacart-policy-bot-vxgrwy2cnvhbvhm8dzzkax.streamlit.app

## Features
- Sirf `policies/` folder ki files se jawab
- Har jawab mein file aur section ka hawala (jaise `[file 01, Section 2.1]`)
- Sawal ke liye zaroori detail na ho to ek clarifying sawal
- Contact date ke hisaab se sirf lagu files use hoti hain
- Prompt injection ka tahaffuz: policy files mein likhi hidayat ko bot ignore karta hai

## Setup
1. Repo clone karo.
2. `pip install -r requirements.txt`
3. `.env` file banao aur usme `GEMINI_API_KEY=your_key` likho.
4. `streamlit run app.py`

## Files
- `app.py`: chat app (Streamlit + Gemini)
- `hello.py`: API connection test
- `policies/`: 22 policy files (organizer ki di hui)
