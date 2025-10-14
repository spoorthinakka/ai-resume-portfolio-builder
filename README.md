# 🧠 AI Resume & Portfolio Builder

Generate an ATS-friendly resume and a matching one-page portfolio site using a Hugging Face LLM—then download as PDF/DOCX/TXT or HTML zip.

## Project Summary
**AI Resume & Portfolio Builder** is a Streamlit app that turns your inputs into a polished, ATS-friendly resume and a simple one-page portfolio website. It collects your contact details, education, skills, projects, internships/experience, publications, and extras, then uses a Hugging Face chat-instruct model to draft a well-structured CV. The app post-processes the output to enforce consistent headings, bullet rules, and clean formatting so you can download professional copies in **PDF, DOCX, or TXT**.

Beyond resumes, the app can export a **mini portfolio site** (HTML + CSS) as a zip based on your final resume content. You can pick visual templates for both the resume and the website, edit the generated text inline, and optionally get a lightweight **ATS/role-fit score** with quick reasons to guide improvements. All secrets are handled via environment variables to keep tokens out of your codebase.

## Key Features
- Streamlit UI covering all core resume sections
- Hugging Face **Inference API** (configurable via \HF_MODEL\)
- Smart cleanup: heading normalization, bullet enforcement, section ordering
- One-click downloads: **PDF**, **DOCX**, **TXT**
- **Portfolio export**: generates \index.html\ + \styles.css\ as a zip
- Optional **ATS / role-fit scoring** with concise feedback
- Secrets via **.env** (\HF_TOKEN\), no tokens in code

## Tech Stack
- **Streamlit** (UI)
- **huggingface_hub** (LLM calls)
- **FPDF** (PDF), **python-docx** (DOCX)
- **python-dotenv** (env config)

