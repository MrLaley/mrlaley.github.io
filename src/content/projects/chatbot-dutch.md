---
title: "AI Chatbot for Learning Dutch"
description: "Development and UX research of a voice-enabled AI web application designed to facilitate Dutch language learning through real-time immersive conversations."
pubDate: "Jan 18 2026"
heroImage: '../../assets/chatbot-dutch-cover.png'
category: "university"
---

## Project Overview

This project focuses on the end-to-end development, UX research, and testing of a voice-enabled AI web application designed to help international students practice speaking Dutch. By simulating real-world scenarios in a judgment-free environment, the application bridges the gap between passive language learning and active conversational fluency. 

The project was driven by a comprehensive User Experience (UX) methodology, progressing from initial problem identification and user interviews to Lo-Fi/Hi-Fi prototyping, and finally to controlled experimental validation.

---

## Technical Architecture & AI Integration

The core product is a mobile-friendly web application that leverages modern AI technologies to create a seamless, real-time spoken interaction:

* **Speech-to-Text (STT):** Captures user audio via FFMPEG and processes it through the Google Speech API to transcribe spoken Dutch into text accurately.
* **Large Language Models (LLMs):** Serves as the cognitive engine of the chatbot. The system employs an advanced **dual-prompting technique**:
  * One prompt strictly maintains the agent's persona and context (e.g., acting as a waiter or doctor).
  * The second prompt analyzes the user's input to generate instructional value, providing live grammatical and pronunciation feedback.
* **Text-to-Speech (TTS):** Converts the AI's generated responses into a natural-sounding Dutch voice, simulating a true conversational partner.
* **Dynamic Contextualization:** Users can select specific contexts (e.g., Grocery Store, Doctor's Appointment) and the AI dynamically adapts its vocabulary and tone to the scenario.

---

## UX Research & Product Development Phases

The product's evolution was strictly guided by empirical data gathered through multiple phases of user testing and iteration.

### 1. Problem Identification & User Interviews
We conducted in-depth interviews with international students to identify primary barriers to learning Dutch. The data revealed that **social anxiety** (fear of making mistakes) and **rigid schedules** were the main obstacles. The insight gained was that users prioritize a "psychologically safe" rehearsal space and extreme flexibility over traditional immersive setups like VR.

### 2. Low-Fidelity (Lo-Fi) Prototyping
Before writing complex code, we tested the core interaction loop using paper prototypes and a "Wizard of Oz" testing methodology. 
* **Findings:** Users highly valued the concept of error correction but rejected manual "tone" selectors. This phase validated that immediate, contextual feedback was the product's main selling point.

### 3. High-Fidelity (Hi-Fi) Prototyping
We developed the fully functional web application integrating the STT, LLM, and TTS pipelines. We introduced a **"Live Feedback"** feature that visually highlights grammatical corrections mid-conversation.
* **Findings:** 100% of non-native participants reported feeling significantly less nervous speaking to the AI than to a real person. However, we discovered that overly verbose feedback disrupted the conversational flow, leading to iterative design improvements focusing on concise, color-coded corrections.

### 4. Controlled Experimentation Design
To statistically validate the effectiveness of the "Live Feedback" feature, we designed a large-scale, Between-Participants controlled experiment. The methodology utilizes Independent Samples T-tests to measure:
* **Grammatical Accuracy:** Objective tracking of syntax errors during a 5-minute session.
* **Speaking Confidence:** Subjective assessment via Likert-scale questionnaires to measure the reduction in social anxiety.

---

## Ethical Considerations & Conclusion

As the prototype moves towards a Minimum Viable Product (MVP), we addressed critical ethical considerations, including **Biometric Bias** (ensuring the AI understands diverse non-native accents) and **Data Privacy** regarding voice recordings. 

Ultimately, this project demonstrates a complete product lifecycle, from identifying a genuine user pain point to engineering a sophisticated, AI-driven solution validated by rigorous UX methodologies.
