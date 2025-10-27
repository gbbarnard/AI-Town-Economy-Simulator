# Japanese Language Tutor Bot

#**Project Overview**

  The Japanese Language Tutor Bot is an AI-powered conversational learning tool designed to help users practice and improve their Japanese language skills.  
It uses a Large Language Model (LLM) to engage in realistic dialogues, correct grammar and vocabulary errors, and explain mistakes in simple English.  

Unlike static language-learning apps, this tutor adapts to the learner’s ability.  
As users make progress, the system automatically adjusts sentence complexity and grammar difficulty based on JLPT (Japanese-Language Proficiency Test) levels.  
Session data are logged for progress visualization and analysis.

#**Problem Statement**

 Traditional language apps rely on pre-set questions and fixed feedback, offering little personalization.  
Learners of Japanese often struggle with context, verb conjugation, and particle usage, making feedback essential.

This project explores whether a conversational AI tutor can:
- Provide instant feedback and correction in real time,  
- Offer brief, human-like explanations, and  
- Adapt its difficulty dynamically to learner performance.  

#**Proposed Method**

 1. **LLM-Driven Conversation Engine**  
   - Build a Streamlit chat interface for Japanese dialogue.  
   - Connect to an LLM API (OpenAI / Anthropic / OpenRouter).  
   - Maintain multi-turn conversations within daily-life topics.

2. **Grammar Correction & Feedback**  
   - Parse each learner message and detect common mistakes.  
   - Return structured JSON
   - Display correction and explanation below the chat window.

3. **Adaptive Difficulty**  
   - Track mastery scores (0 – 100) per grammar category.    
   - Adjust grammar and vocabulary difficulty automatically.

4. **Session Logging & Visualization**  
   - Log each exchange as JSON (user input, correction, topic, mastery).  
   - Plot progress and error trends with Matplotlib / Altair.

#**Data Sources**

- Synthetic data only (generated from simulated learner sessions).  
- Stored in `/logs/sessions/` as JSON for evaluation. 
