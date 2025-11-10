# AI Resume & Portfolio Builder  
👉 [**Live Demo on Streamlit**](https://ai-resume-and-portfolio-builder.streamlit.app)

Generate an ATS-friendly resume and a matching one-page portfolio site using a Hugging Face LLM — then download as **PDF**, **DOCX**, **TXT**, or **HTML zip**.

---

## Project Summary
**AI Resume & Portfolio Builder** is a Streamlit web app that turns your inputs into a polished, ATS-friendly resume and a simple one-page portfolio website. It collects your contact details, education, skills, projects, internships/experience, publications, and extras, then uses a Hugging Face chat-instruct model to draft a well-structured CV. The app post-processes the output to ensure clean formatting, consistent headings, and neat bullet points, allowing you to download professional copies in **PDF**, **DOCX**, or **TXT** formats. Beyond resumes, the app can export a **mini portfolio site** (HTML + CSS) as a zip file based on your final resume content. You can pick visual templates, edit the generated text inline, and optionally get a lightweight **ATS / role-fit score** with improvement suggestions. All secrets are handled via environment variables to keep tokens secure.

---

## Key Features
- Streamlit UI covering all core resume sections  
- Hugging Face **Inference API** (configurable via `HF_MODEL`)  
- Smart cleanup: heading normalization, bullet enforcement, section ordering  
- One-click downloads: **PDF**, **DOCX**, **TXT**  
- **Portfolio Export**: generates `index.html` + `styles.css` as a zip  
- Optional **ATS / role-fit scoring** with concise feedback  
- Secrets via `.env` (`HF_TOKEN`), no tokens stored in code  

---

## Tech Stack
- **Streamlit** – Interactive web interface  
- **Hugging Face Hub** – LLM-based resume drafting  
- **FPDF** – PDF generation  
- **python-docx** – DOCX file export  
- **python-dotenv** – Environment variable management  

---

## Deployment
You can try the live app here:  
👉 [**AI Resume & Portfolio Builder on Streamlit**](https://ai-resume-and-portfolio-builder.streamlit.app)

This project is deployed using **Streamlit Cloud**, allowing users to instantly generate and download AI-crafted resumes and portfolio websites directly from their browser (no setup required).

---

## License
This project is licensed under the [MIT License](./LICENSE).  
Feel free to use and modify it with proper credit.
