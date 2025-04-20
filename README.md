# Debate.AI — Train Your Mind to Win the Argument

> **"Tired of losing couch debates on Twitter? Or do you struggle to remember a vital argument during a real dispute on time?"**

> **"We present a solution just for you!"**

> **"Enrich your debate skills with Debate.AI — a Google Gemini-based service."**

---

## 🧠 The Use Case

In today’s fast-paced world, the ability to argue clearly, respond to counterpoints, and structure thoughts under pressure is more valuable than ever — whether you're a student, content creator, public speaker, or just someone who enjoys a good discussion.

**But good debate requires practice.** And practicing debates with real people is rarely consistent, structured, or measurable.

That’s where Debate.AI comes in.

---

## 🎯 The Problem

While conversational AI is becoming more accessible, **debate simulation remains largely unexplored**. The typical AI assistant lacks structure, adversarial positioning, and dynamic role management.

We wanted to solve:
- The lack of debate-specific practice tools
- The absence of grounded, real-time counterarguments
- The need for immersive, audio-supported interactions
- The inability to measure improvement with AI-driven evaluation

---

## 🚀 Our Solution: Debate.AI

Debate.AI is a fully autonomous debate simulator that brings together:
- 💬 An intelligent opponent powered by Google Gemini
- 🎙️ Text-to-speech voices to bring personalities to life
- 🧠 Live topic grounding via web search
- 📊 Structured scoring and performance feedback
- 🔄 Role-switching state machine that simulates debate dynamics

With each session, users go head-to-head with an AI opponent over a randomly selected topic. The debate is moderated by another AI that provides context, manages the flow, and evaluates responses.

> 📸 _Placeholder for live session screenshot_  
> `![Debate Session](./images/debate_sample.jpg)`

---

## 🧭 How the Debate Unfolds: Stage by Stage

Debate.AI isn’t just back-and-forth chatter — it follows a structured, multi-phase format to simulate real debate dynamics and ensure depth in every session:

### **Stage 1: Opening Statements**
Each opponent presents their perspective based on their assigned stance.  
The moderator invites both the human and AI opponent to share their initial arguments.  
If a speaker provides vague or meaningless input, the moderator flags it and prompts them to try again.

### **Stage 2: Moderator's Inquiry**
The moderator poses targeted questions to each opponent, addressing any missing logic, weak points, or vague claims from their opening statements.  
Up to 5 questions per opponent are allowed.  
Each speaker then responds with clarification, elaboration, or defense.

### **Stage 3: Cross-Examination**
Now it’s the opponents' turn to challenge each other.  
Each asks up to 3 questions aimed at poking holes in the other's logic or strengthening their own case.  
They respond in kind, defending their positions under pressure.

> 📸 _Placeholder for debate timeline or flowchart_  
> `![Debate Flow](./images/debate_stages.jpg)`

---

## 🛠️ Technologies Used (Tech Stack)

The project combines several cutting-edge GenAI technologies and tools:

### 🧠 **Google Gemini (via `google-genai` & `langchain-google-genai`)**
Used for generating arguments, moderator content, and structured outputs.  
**Capabilities:** Few-shot prompting, function calling, long context, evaluation.

### 🕸️ **LangGraph**
Manages the multi-role flow (moderator → human → opponent → repeat) via a visual and functional state machine.  
**Capabilities:** Agents, structured orchestration.

### 📚 **ChromaDB + Custom Embeddings**
Stores and retrieves debate content and contextual data using Gemini-powered text embeddings.  
**Capabilities:** Embeddings, vector database, retrieval-augmented generation (RAG).

### 🔍 **Google Search Tool**
Gemini’s tool-calling is used to retrieve fresh, live information on complex topics, grounding the AI’s arguments in reality.  
**Capabilities:** Grounding, function calling.

### 🎤 **Kokoro ONNX (TTS)**
Each speaker (moderator, opponent) has a unique voice generated via Kokoro models, turning text responses into lifelike audio.  
**Capabilities:** Audio understanding, voice synthesis.

### 🧪 **Structured Enum-Based Evaluation**
Arguments are scored using Gemini-generated structured output — from “Very Bad” to “Very Good” — returned in a standardized JSON schema.  
**Capabilities:** Structured output, GenAI evaluation.

---

## ⚙️ How It Works

1. **Topic Generation:** Randomly selects a thought-provoking topic from a curated list.
2. **Contextual Grounding:** Performs a web search and builds a knowledge corpus using Gemini.
3. **Corpus Embedding:** Splits and stores that information in a vector DB using custom embeddings.
4. **Stateful Debate Flow:** Uses LangGraph to manage structured, turn-based interactions between participants.
5. **Response Scoring:** Each human response is evaluated by Gemini using a prompt-based rubric and scored automatically.
6. **Audio Output:** Responses are spoken using AI-generated voices to simulate a real debate experience.

> 📸 _Placeholder for system architecture diagram_  
> `![System Architecture](./images/system_architecture.jpg)`

---

## ✅ GenAI Capabilities Demonstrated

This project demonstrates **9 GenAI capabilities** required by the capstone:

✅ Structured Output
✅ Grounding
✅ Agents
✅ Embeddings  
✅ Retrieval-Augmented Generation
✅ Vector Database  

---

## 🔬 Reflections & Learnings

**What worked well:**
- LangGraph enabled modular role control and clean state transitions
- Voice output made debate immersive and realistic
- Structured scoring gave users immediate feedback on quality

**Challenges:**
- Gemini’s search grounding can occasionally miss niche arguments
- Evaluation logic could benefit from reinforcement learning
- Interface is still notebook-based — we plan to build a web UI

---

## 📍 What's Next

- 🌐 Launch a web version with real-time interaction
- 👥 Enable human vs human or peer challenges
- 💬 Custom topic creation with bias control
- 🧭 Replay mode with annotated feedback

---

## 📣 Final Thoughts

Debate.AI is more than a chatbot — it’s a **thinking partner**, a **rhetorical sparring coach**, and a **use case of GenAI** that blends voice, structure, grounding, and evaluation into one experience.

We hope it inspires others to explore intelligent simulation tools for communication training, education, and even entertainment.

---

## 🔗 Competition Link

This project was created as part of the [Gen AI Intensive Course Capstone 2025Q1](https://www.kaggle.com/competitions/gen-ai-intensive-course-capstone-2025q1).

> 📸 _Placeholder for CTA or Try it now_  
> `![Try Debate.AI](./images/try_now.jpg)`

---

Thanks for reading — and see you in the debate ring.

**– The Debate.AI Team**
