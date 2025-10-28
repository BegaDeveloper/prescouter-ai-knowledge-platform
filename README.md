# 🧠 PreScouter – AI-Powered Knowledge & Research Platform (USA)

## 🚀 Introduction

**PreScouter** is an **AI-driven research and knowledge management platform** developed for enterprise clients in the USA, enabling organizations to **leverage internal and external data** through interactive, ChatGPT-style AI interfaces.
The system allows users to **upload documents, files, and datasets**, train multiple chat models for specific purposes, and **interactively query organizational knowledge** to accelerate research and decision-making.

Designed for innovation teams, R&D departments, and corporate analysts, PreScouter’s platform transforms how users **search, learn, and collaborate with data** — all powered by a scalable, modular web architecture.

---

## 🧩 What the App Does

PreScouter serves as a **central AI knowledge hub** where companies can consolidate and interact with their research materials in real time.
The app enables users to:

* 💬 **Create AI chat models** specialized for different topics or data sets.
* 📂 **Upload and analyze large data files** (PDFs, Word, Excel, etc.).
* 🧠 **Train models** on internal knowledge bases to produce tailored insights.
* 🔎 **Search and query data conversationally** using AI-powered retrieval.
* 🔄 **Collaborate** across research teams, sharing chats and learned data securely.

Its intuitive ChatGPT-like interface and modular design made it easy for users to build and manage multiple knowledge agents under a single workspace.

---

## 🧠 Technologies Used

| Layer                           | Stack / Tools                                                                              | Description                                                                                       |
| ------------------------------- | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------- |
| **Frontend**                    | **Angular 18**, **Nx Monorepo (Microfrontends)**, **RxJS**, **Angular Material**, **SCSS** | Built a modular, scalable front-end for multi-instance chat models and real-time AI interactions. |
| **Backend**                     | **Express.js (Node.js)**                                                                   | Managed APIs, authentication, and AI processing logic for chat sessions and file data ingestion.  |
| **Database / Cloud**            | **Firebase (Auth, Firestore, Storage)**                                                    | Stored user data, trained models, and chat histories securely.                                    |
| **Deployment / Infrastructure** | **Google Cloud Platform (GCP)**                                                            | Hosted the backend and enabled secure API communication.                                          |

---

## 💻 My Role & Contributions

I worked as a **Senior Angular Developer**, responsible for designing and developing the **frontend architecture** and ensuring a smooth integration between the Angular app, Firebase services, and the AI backend.

While the initial system was built as a single large Angular app, I led the **mid-project migration to a microfrontend architecture using Nx**, which allowed different AI modules (chat interface, file management, knowledge training, admin panel) to run independently yet share common libraries and state logic.

Key contributions:

* Designed and implemented **Angular Nx-based microfrontend structure** mid-development without downtime.
* Created **modular AI chat components** supporting dynamic model selection, file uploads, and real-time streaming responses.
* Integrated **Firebase Auth and Firestore** for secure user sessions and chat persistence.
* Built reusable **UI modules and shared libraries** to unify styles and interactions across different AI chat apps.
* Collaborated with backend engineers to define **Express.js endpoints** for AI query execution and knowledge ingestion.

---

## ⚙️ Challenges & Solutions

### 🧩 1. Implementing Microfrontends Mid-Development

One of the biggest challenges was introducing **Nx microfrontends** halfway through the project — after several modules had already been built in a monolithic Angular structure.

I solved this by:

* **Refactoring existing features into Nx libraries** (shared, core, UI, and services).
* Creating separate **apps** for each AI module (Chat, Knowledge Base, Admin, Insights).
* Establishing a **common interface library** for shared types, models, and route contracts.
* Using **Module Federation** to load remote apps dynamically without code duplication.

This transition improved scalability, reduced build time, and allowed teams to work in parallel without merge conflicts — all while keeping the app stable in production.

---

### ⚙️ 2. Real-Time Data Flow & Chat Synchronization

AI conversations and model training required **live data synchronization** between the frontend and backend.
I implemented a **real-time event stream layer** using RxJS and WebSocket-like patterns that:

* Streamed AI-generated responses incrementally.
* Handled concurrent chat updates between multiple sessions.
* Persisted chat history instantly to Firestore for seamless reloads.

This ensured that users always received **low-latency, real-time AI interactions** — similar to ChatGPT’s typing behavior.

---

### ⚙️ 3. File Upload & Knowledge Training Pipeline

Users could upload research papers, presentations, or reports to teach their custom chat models.
I developed the **frontend file ingestion module** that:

* Uploaded files to Firebase Storage with progress indicators.
* Sent file metadata to the Express backend for AI processing.
* Managed file status and errors with NgRx and centralized notifications.

This modular upload system allowed **batch uploads and background processing**, improving user workflow and reliability.

---

## 🧩 What We Built

* **Multi-Chat AI Interface** – ChatGPT-style UI for users to run multiple AI models simultaneously.
* **File Upload & Knowledge Training** – File ingestion pipeline to train AI models on user data.
* **AI Knowledge Hub** – Searchable database for organizational research content.
* **Microfrontend Workspace** – Modular Nx structure enabling multiple Angular apps under one ecosystem.
* **Secure Firebase Auth & Storage** – Role-based access, persistent chat logs, and safe data handling.

---

## 🏁 Outcome

The PreScouter AI platform evolved into a **powerful enterprise research assistant**, enabling companies to centralize knowledge, upload and train their own data, and interact through intelligent conversational agents.
The **microfrontend migration** and **Firebase integration** made the app **scalable, secure, and flexible**, setting the foundation for future AI-driven knowledge tools used across multiple industries.

