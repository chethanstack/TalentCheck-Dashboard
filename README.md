# 🎯 TalentCheck Dashboard

> ## 📌 Portfolio Notice
>
> This repository is my **personal portfolio copy** of a team hackathon project, published with permission from the team lead.
>
> The project was collaboratively developed by a team of five members. This repository is intended to showcase my contributions while giving full credit to all team members. The original project remains the collaborative work of the entire team.
>
> **AI-assisted development** was used during the hackathon to accelerate implementation. All features were integrated, tested, reviewed, and validated by the team.

<p align="left">
  <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/FastAPI-Backend-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI">
  <img src="https://img.shields.io/badge/JavaScript-Frontend-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/Status-Hackathon%20MVP-orange?style=for-the-badge" alt="Status">
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License">
</p>

TalentCheck Dashboard is an all-in-one HR-tech solution designed to optimize the recruitment workflow. By leveraging automation and intelligent analysis, this platform helps recruiters and candidates connect faster and more effectively by providing data-driven insights into candidate readiness for specific roles.

---

# ✨ Core Features

| Feature                | Description                                                                                                            |
| :--------------------- | :--------------------------------------------------------------------------------------------------------------------- |
| 📄 **JD Analysis**     | Automatically parses Job Descriptions (PDF/DOCX) and extracts required skills mapped to the 12 RADIX skill categories. |
| 📑 **Resume Parsing**  | Converts unstructured PDF/Word resumes into structured, comparable candidate data.                                     |
| 👤 **Profile Builder** | Auto-populates candidate profiles from parsed resumes with additional editable information.                            |
| ✅ **Talent Check**     | Calculates readiness scores, candidate tiers, and improvement areas based on company and role requirements.            |
| 🔍 **Skill Matching**  | Compares candidate skills against uploaded job descriptions and identifies matched and missing skills.                 |

---

# 🛠️ Tech Stack

| Layer                 | Technology                                            |
| :-------------------- | :---------------------------------------------------- |
| **Frontend**          | HTML5 + Vanilla JavaScript (Fetch API)                |
| **Backend**           | Python 3 + FastAPI + Uvicorn                          |
| **Data Storage**      | JSON (Hackathon MVP)                                  |
| **Resume/JD Parsing** | pdfplumber, python-docx                               |
| **Skill Extraction**  | Rule-based keyword mapping across 12 RADIX categories |
| **Fuzzy Matching**    | RapidFuzz                                             |
| **Validation**        | Pydantic                                              |

> **Why no LLM API in the MVP?**
>
> The MVP intentionally uses deterministic keyword and section-based extraction to ensure fast, explainable, offline-friendly execution with no dependency on external AI APIs during demonstrations. The extraction layer is modular, making future integration with LLMs straightforward.

---

# 🚀 Getting Started

## Prerequisites

* Python 3.10+
* Git

## Installation

```bash
git clone https://github.com/chethanstack/JD_Analytics.git
cd JD_Analytics
```

```bash
cd backend
pip install -r requirements.txt
```

```bash
uvicorn main:app --reload --port 8000
```

Open `frontend/index.html` in your browser (or use any static web server). The frontend communicates with `http://localhost:8000`.

---

# 📖 Quick Usage

1. Upload a Job Description.
2. Upload a Resume.
3. Complete the remaining profile information.
4. Run Talent Check.
5. View readiness score and recommendations.
6. Compare skills with the uploaded Job Description.

---

# 📂 Project Structure

```text
TalentCheck-Dashboard/
├── backend/
│   ├── main.py
│   ├── requirements.txt
│   ├── data/
│   └── services/
├── frontend/
│   └── index.html
└── README.md
```

---

# 👨‍💻 My Contribution

My primary responsibility in this project was the **Job Description Analysis** module.

Contributions include:

* Implemented the Job Description Analysis workflow.
* Developed PDF/DOCX job description parsing.
* Built the skill extraction pipeline.
* Mapped extracted skills into the 12 RADIX skill categories.
* Integrated the module with the overall application workflow.
* Participated in testing, debugging, and team integration during the hackathon.

---

# 👥 Project Team

This project was collaboratively developed by:

| Module          | Contributor      |
| :-------------- | :--------------- |
| JD Analysis     | **S. Chethan**   |
| Resume Parsing  | I. Mahesh Reddy  |
| Profile Builder | A. Indra Varshit |
| Talent Check    | N. Thulasi Ram   |
| Skill Matching  | J. Jaswanth      |

---

# 🤖 AI-Assisted Development

This project was developed during a hackathon using AI-assisted development tools alongside manual software engineering, debugging, testing, and feature integration by the team.

AI tools were used to accelerate development while the implementation, validation, and final integration remained the responsibility of the project team.

---

# 🙏 Acknowledgement

This repository is maintained as my personal portfolio copy with permission from the team lead.

Credit goes to all team members for their respective contributions throughout the hackathon.

---

# 📄 License

This repository is shared for educational and portfolio purposes.

If you wish to reuse significant portions of the project, please contact the contributors first.
