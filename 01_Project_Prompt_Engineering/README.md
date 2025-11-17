# AI Career Advisor (Prompt Engineering)

## Project Overview
This project is a simple LLM-based chatbot that provides career guidance for students and freshers. The chatbot is built using **prompt engineering only** — no external data sources are used.

**Goal:** Help students with learning paths, resume improvement, and career advice in a clear, structured, and beginner-friendly manner.

---

## Objective
- Build a simple LLM-powered chatbot.
- Use structured prompts to define the model as a "Career Advisor".
- Guide students with practical and positive suggestions.
- Keep responses concise (4–6 lines) and easy to understand.

---

## Prompt Design

1. **Role-based Prompt (System Prompt)**  
Defines the chatbot’s role:  
> You are an expert Career Advisor who guides students with clear, positive, and practical career suggestions.  
> You must avoid giving false information and only provide helpful, realistic, and encouraging advice.

2. **Instruction-based Prompt**  
Describes the task:  
> Your task is to help beginners choose learning paths, improve resumes, and suggest career options.  
> Your answers should be short, simple, and easy for students to understand.

3. **Few-shot Example Prompt**  
Provides example interactions to set response style:  
> **User:** I am interested in web development, where should I start?  
> **Assistant:** Start with HTML, CSS, and JavaScript. After basics, learn React or Vue. Practice by building small projects like portfolio website, todo app, or landing pages.  

> **User:** How can I improve my resume as a fresher?  
> **Assistant:** Keep it one page, add education, skills, personal projects, and GitHub links. Avoid long paragraphs.

---

## Test Queries & Sample Outputs

| Query | Sample Output |
|-------|---------------|
| I am in my 1st semester. How should I start coding? | Begin with Python or C, practice variables, loops, and arrays. Build small programs like a calculator or sorting tool. Then try small projects. |
| How can I make my resume strong? | Keep it one page. Add education, skills, and 2–3 mini projects. Include GitHub links and use bullet points. |
| Web development roadmap? | Start with HTML → CSS → JavaScript. Then learn React or Node.js. Make projects: portfolio, ecommerce UI, todo app. |
| Data Science path? | Learn Python, NumPy, Pandas, Matplotlib, statistics. Then learn ML basics like regression and classification. Practice Kaggle datasets. |
| Internship without experience? | Work on projects and upload to GitHub. Apply on LinkedIn daily. Keep resume concise. Seek guidance from seniors and participate in hackathons. |

---

## Before vs After Prompt Optimization

- **Before:** Long, confusing answers; generic resume advice; sometimes unrelated suggestions.  
- **After:** Concise, structured, beginner-friendly guidance; step-by-step instructions; career-context focused; no hallucinations.

---

## Deliverables

- `career_advisor.ipynb` – The Jupyter Notebook with all prompts and test outputs.  
- `career_advisor.md` – Project report summarizing prompt design and observations.

---

## Conclusion
This project demonstrates that **prompt engineering alone** can produce a reliable, beginner-friendly AI Career Advisor. Optimized prompts result in concise, accurate, and structured guidance without relying on external data.
