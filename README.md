Prerequisites

1. Download and install pycharm (python editor)

https://www.jetbrains.com/pycharm/download/?section=windows


2. install UV Packaage manager

https://docs.astral.sh/uv/getting-started/installation/#installation-methods

3. Get Gemini API key

<img width="730" height="139" alt="image" src="https://github.com/user-attachments/assets/6f6ac4a6-7b84-401c-9985-27f111fb612e" />


 4. Craete project

 uv init crewai-ananthan

5. Open project in pycharm

6. add crew packge

# uv add crewai[tools]

6. Configure Interpreter:
 
 check interpreter is present under our virtual environment
 
 .venv --> scripts directory

<img width="304" height="269" alt="image" src="https://github.com/user-attachments/assets/a8fd3358-7b0b-4455-aa82-c0cd71e475a5" />

7. check the interpreter is loaded, if not choose add interpreter and imprort the interpreter from local
file --> settings

<img width="881" height="362" alt="image" src="https://github.com/user-attachments/assets/ec0814c7-fcd6-4785-b45c-fbb6261df782" />

**Setup First Agant**

1. Right click on project --> new -->Jupyter Notebook and set agent name "1_email_agent"

   <img width="578" height="155" alt="image" src="https://github.com/user-attachments/assets/b9bbb79e-f699-4c1b-9279-d57eea711f82" />

   <img width="633" height="257" alt="image" src="https://github.com/user-attachments/assets/9fa7732c-73a8-4711-8d70-fe2b609a52c4" />

2. Validate the file craetion

   <img width="317" height="220" alt="image" src="https://github.com/user-attachments/assets/3b0ca86c-5043-4e01-8e07-bad11d4963cc" />

3. To add gemini API key, craete .env file under venv(virtual enviroenmnet folder)

<img width="730" height="139" alt="image" src="https://github.com/user-attachments/assets/02be7df0-f759-49be-95c7-bf17039a5bad" />

5. Validate the API key by loading env

- ENV var load

from dotenv import load_dotenv
load_dotenv()

import gemini to crewai

"from crewai import LLM
llm = LLM (
    model="gemini/gemini-2.0-flash",
    temperature=0.1
)
llm.call("who is CEO of publicissapient.") "



   <img width="920" height="370" alt="image" src="https://github.com/user-attachments/assets/3e338802-0f0a-44ae-80f9-c2dc4699c65e" />

   <img width="900" height="342" alt="image" src="https://github.com/user-attachments/assets/6e2a45d4-c2a4-46f5-9272-2502b252469e" />





  














**Notes:**

1. What is an Interpreter?

An interpreter is a program that directly executes code line by line (or statement by statement), without converting the whole program into machine code in advance.

Unlike a compiler (which translates the entire source code into machine code first), an interpreter reads, analyzes, and runs the code on the fly.

2. What is Jupyter Notebook?

Jupyter Notebook is an open-source, interactive web application that lets you:

Write and run code (Python, R, Julia, and more).

Add text/notes (with Markdown).

Visualize data (charts, plots, dashboards).

Mix everything into one document.

It runs in your browser but executes code on your local machine (or a server, like JupyterHub, Google Colab, or cloud platforms).

🔑 The name Jupyter comes from Julia + Python + R.
