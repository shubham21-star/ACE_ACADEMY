<!-- 🌟 AI Handbook Assistant using RAG by Shubham Kumar -->

<h1 align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=00FFB3&center=true&vCenter=true&width=700&lines=Welcome+to+AI+Handbook+Assistant+using+RAG!;Beginner-Friendly+AI+Project+🤖;Created+by+Shubham+Kumar+💻" alt="Typing SVG" />
</h1>

---

<p align="center">
  <img src="https://img.shields.io/badge/Language-Python-blue.svg?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Platform-Google%20Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white" />
  <img src="https://img.shields.io/badge/AI-RAG-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Track-B%20RAG%20%26%20Knowledge-purple?style=for-the-badge" />
</p>

---

# 🧭 About Project

This project is a **beginner-level AI application** based on the concept of **Retrieval Augmented Generation (RAG)**.

The AI Handbook Assistant retrieves answers from handbook data and displays relevant responses based on user questions.

💡 *This project is simple, easy to understand, and perfect for beginners learning Prompt Engineering and AI concepts.*

---

# 🚀 Features

- ✅ Beginner-Friendly Project  
- ✅ Simple Python Implementation  
- ✅ Retrieval-Based AI Assistant  
- ✅ Prompt Engineering Included  
- ✅ Google Colab Compatible  
- ✅ Handbook-Based Question Answering  

---

# 📂 Project Structure

| File | Description |
|------|-------------|
| `main.py` | Main Python program |
| `handbook.txt` | Knowledge base / handbook data |
| `README.md` | Project documentation |

---

# ⚙️ Technologies Used

| Technology | Purpose |
|------|----------|
| 🐍 Python | Main Programming Language |
| 📘 Google Colab | Development Platform |
| 📄 Text File | Knowledge Storage |
| 🤖 Prompt Engineering | AI Instructions |
| 🧠 RAG Concept | Retrieval-Based Answers |

---

# 🧠 Concepts Used

- ✅ Artificial Intelligence  
- ✅ Prompt Engineering  
- ✅ Retrieval Augmented Generation (RAG)  
- ✅ File Handling  
- ✅ User Input Handling  
- ✅ Information Retrieval  

---

# 🔄 Project Workflow

```text
User Question
      ↓
Read Handbook Data
      ↓
Search Matching Information
      ↓
Retrieve Relevant Answer
      ↓
Display Output
```

---

# 💻 Main Python Code

```python
print("===================================")
print(" AI Handbook Assistant using RAG ")
print("===================================")

while True:

    question = input("\nAsk your question (type exit to quit): ")

    if question.lower() == "exit":
        print("\nThank You!")
        break

    found = False

    print("\nSearching handbook...\n")

    for line in data:

        if question.lower() in line.lower():

            print("Answer:")
            print(line)

            found = True

    if found == False:
        print("The handbook does not contain this information.")
```

---

# 📄 Sample Handbook Data

```text
Artificial Intelligence (AI) is the simulation of human intelligence by machines.

Machine Learning is a branch of AI.

Python is a popular programming language.

RAG stands for Retrieval Augmented Generation.

Prompt Engineering is used for designing effective AI prompts.
```

---

# ▶️ How to Run

Run the project in **Google Colab**:

```python
# Run all cells one by one
```

Then ask questions like:

```text
AI
Python
RAG
Prompt Engineering
```

To stop:

```text
exit
```

---

# 📊 Evaluation Test Cases

| Query | Expected Result | Status |
|------|-----------------|--------|
| AI | AI Definition | ✅ Pass |
| Python | Python Information | ✅ Pass |
| RAG | RAG Meaning | ✅ Pass |
| IPL Score | Refusal | ✅ Pass |
| Bitcoin | Refusal | ✅ Pass |

---

# 🔐 System Prompt

```python
SYSTEM_PROMPT = """
You are an academic handbook assistant.

Rules:
1. Answer only from handbook data.
2. Give short and simple answers.
3. If answer is not found, say:
   'The handbook does not contain this information.'
"""
```

---

# 🔰 Future Improvements

- ✅ Add GUI Interface  
- ✅ Upload PDF Support  
- ✅ Add Real AI APIs  
- ✅ Improve Retrieval Accuracy  
- ✅ Voice Assistant Integration  

---

# 👨‍💻 Author

<p align="center">
  <img src="https://avatars.githubusercontent.com/shubham21-star" width="120" style="border-radius:50%;" alt="Shubham Kumar Avatar"/>
</p>

<p align="center">
  <b>Shubham Kumar</b><br>
  💻 B.Tech Data Analytics Student<br>
  🤖 AI & Data Analytics Enthusiast<br>
  🌐 <a href="https://github.com/shubham21-star" target="_blank">GitHub Profile</a>
</p>

---

# ✨ Conclusion

The AI Handbook Assistant using RAG is a simple and beginner-friendly AI project developed using Python and Google Colab.

This project demonstrates:
- Prompt Engineering
- Retrieval-Based AI
- Knowledge Search
- Beginner-Level RAG Concepts

It is useful for understanding how AI assistants retrieve and display relevant information from stored documents.

---

# 🌟 Quote

> “AI is not just about generating answers — it is about retrieving the right knowledge.” 🤖

---

<p align="center">⭐ From <b>Shubham Kumar</b> with ❤️</p>