# Smart India Hackathon Workshop
# Date:07-04-2025
## Register Number:212224230049
## Name:DAKSHINA MOORTHY N D
## Problem Title
SIH 1653: Web based Selector-Applicant Simulation Software
## Problem Description
Background: Recruitment and Assessment Centre (RAC) under DRDO, Ministry of Defence carries out interviews for applications received against advertised vacancies and for promotion to next higher grade for scientific manpower inducted within DRDO. Description: The process of interviewing is a challenging task. An unbiased objective interviewing process helps identify the right talent. The basic process of an interview involves posing a set of questions by an interviewer and thereafter evaluating responses from candidates. Thus, the questions asked should be relevant and match the area/ expertise of the applicant and the responses should also be of relevance w.r.t. the question asked. Expected Solution: The proposed solution should provide experts as well as candidates a real life Board Room experience, starting with initial ice-breaking questions leading to in-depth techno-managerial (depending on the level of candidate) questions. It shall also be able to provide a quantifiable score for experts as well as the candidate for the relevancy of questions w.r.t. the area/ expertise of the applicant. Similarly, candidate responses should also be graded for relevancy w.r.t. the question asked, finally assisting in arriving at an overall score for the subject knowledge of the candidate and thus his/ her suitability against the advertised post.

## Problem Creater's Organization
Ministry of Defence

## Idea

**AI-Powered Web-Based Interview Simulation Platform**

Build an intelligent, web-based platform that **simulates real-life board-room interviews** between selectors and applicants. The platform uses **Artificial Intelligence and Natural Language Processing (NLP)** to dynamically:

- **Generate domain-specific interview questions** tailored to each candidate’s expertise
- **Evaluate candidate responses** for accuracy, relevance, and depth
- **Score both questions and answers** based on alignment with job roles and scientific domains

It provides a **realistic, interactive interview environment** with features like voice/chat interfaces, expert dashboards, and smart analytics — helping RAC/DRDO ensure **unbiased, efficient, and scalable candidate assessments**.

## Proposed Solution / Architecture Diagram
![ChatGPT Image Apr 7, 2025, 05_54_37 PM](https://github.com/user-attachments/assets/ab192976-c7d7-49d0-9f0f-015d09079e12)

## Use Cases


### 1. **Candidate Simulation Experience**
**Goal:** Allow candidates to experience realistic interviews  
- Login to the platform and complete profile
- AI reads resume and infers area of expertise
- System conducts interview with:
  - Ice-breaker questions
  - Technical/domain-specific questions
  - Techno-managerial (for senior candidates)
- Receives score and feedback on performance


### 2. **Expert/Selector Evaluation Panel**
**Goal:** Assist interviewers in conducting and evaluating interviews  
- View candidate background and expertise
- Approve or edit AI-generated questions
- Observe live candidate responses (chat/voice)
- View real-time evaluation from AI
- Give final remarks and scoring


### 3. **AI Question Generator**
**Goal:** Automatically create personalized, relevant interview questions  
- Understand candidate’s domain via resume parsing
- Generate questions across levels (easy to advanced)
- Ensure questions match DRDO’s technical expectations


### 4. **AI Answer Evaluation System**
**Goal:** Automatically assess the quality of candidate responses  
- Use NLP to check:
  - Relevance
  - Completeness
  - Technical depth
- Score and tag responses for expert review


### 5. **Admin & HR Panel**
**Goal:** Manage and monitor the entire interview process  
- Manage candidate & expert user accounts
- Track interview status and progress
- Export scores, reports, feedback
- View analytics (e.g., average scores, department trends)


### 6. **Report Generation**
**Goal:** Create structured reports for each candidate  
- Summary of questions asked
- AI + expert response scores
- Final recommendation for hiring or promotion
- Downloadable PDF or online viewing


## Technology Stack

### **Frontend – What users see**
- **React.js** – Makes the website fast and interactive  
- **Tailwind CSS** – Makes the website look clean and nice  
- **Socket.io** – Helps update things live (like chat or status)  
- **WebRTC** – Lets users talk via voice/video (if needed)


### **Backend – What runs in the background**
- **Python (FastAPI or Django)** – Brain of the system, connects everything  
- **AI Tools (like ChatGPT or BERT)** – Used to create questions and check answers  
- **Machine Learning Tools** – Helps score how good the answers are


### **Database – Where data is stored**
- **PostgreSQL** – Stores user info, scores, etc.  
- **MongoDB** – Stores interview chats and records  
- **Cloud Storage** – Stores resumes, files, or audio recordings


### **Security – Keeps it safe**
- **Login System (JWT)** – Makes sure only the right people can enter  
- **Password Protection (bcrypt)** – Keeps passwords secure  
- **Roles** – Gives different access to candidates, experts, admins


### **Deployment – How it's put online**
- **Docker** – Packs the app so it runs anywhere  
- **GitHub Actions** – Automatically updates the app  
- **Cloud Hosting (like AWS)** – Runs the app on the internet  
- **Nginx** – Helps manage traffic and speed


## Dependencies


### **AI & NLP (Understanding language and scoring)**
- **spaCy** – Reads and understands resumes  
- **Hugging Face Transformers** – Powers smart AI like BERT or GPT  
- **SentenceTransformers** – Checks how well an answer matches a question  
- **OpenAI API** – (Optional) For smart question generation and response checking


### **Machine Learning & Scoring**
- **scikit-learn** – Helps build and train simple models  
- **PyTorch / TensorFlow** – Runs AI models behind the scenes  
- **BERTScore** – Scores the quality of candidate answers


### **Database & Backend Helpers**
- **PostgreSQL / MongoDB** – Save data like profiles, questions, and scores  
- **SQLAlchemy** – Makes it easier to talk to the database using Python


### **Web Development**
- **FastAPI / Django** – Powers the backend and connects everything  
- **React.js** – Builds the user interface  
- **Tailwind CSS** – Makes the website look nice  
- **Socket.io** – For live chat or updates  
- **WebRTC** – (Optional) For live video/voice interview


### **Voice & Speech (Optional)**
- **Whisper / SpeechRecognition** – Converts speech into text  
- **pyaudio** – Handles microphone input/output


### **Security & Auth**
- **JWT / OAuth2** – Keeps user login secure  
- **bcrypt** – Encrypts passwords for safety


### **DevOps & Deployment**
- **Docker** – Packages the app so it runs anywhere  
- **GitHub Actions / Jenkins** – Automates testing and updates  
- **AWS / Azure / GCP** – Runs the app on the cloud


