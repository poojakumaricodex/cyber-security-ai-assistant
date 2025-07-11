# Cybersecurity AI Assistant: Open-Source Cyber Security Assistant 📉

## 🧠 AI Assistant Overview
### Link for the application

https://pooja-2025-cybersecurityassistant.hf.space/?logs=container&__theme=dark&deep_link=NjtmKN94JMg

### **Assistant Name**: Cybersecurity AI Assistant

### **Purpose & Target Audience**
Cybersecurity AI Assistant is designed to serve as an informative assistant focused on **cybersecurity awareness and education**. It targets:

- Students exploring cybersecurity basics
- Non-technical users seeking safety tips
- Beginners learning about digital threats
- Anyone who needs help understanding real-world cyber issues

### **Key Features**
- Answers cybersecurity-related queries
- Explains online safety measures and best practices
- Uses the **"TinyLlama/TinyLlama-1.1B-Chat-v1.0"** model for lightweight inference
- Simple and intuitive interface via **Gradio**
- Generates coherent and context-aware responses to security concerns

---

## 📜 System Prompt Design and Justification

### **Full System Prompt (Embedded in Code)**
```python
prompt = f"User: {{user_input}}\nAssistant:"
```

### **Justification and Impact Analysis**

#### **Breakdown of Elements**
- `"User: {user_input}"`: Identifies user input clearly to set conversational context.
- `"Assistant:"`: Signals the model to generate a response in the assistant’s persona.

#### **Design Choices**
- **Minimalistic structure** encourages concise, contextual, and natural language replies.
- Using `"Assistant:"` sets a role-based expectation that guides TinyLlama to follow a friendly, helpful tone.
- **Temperature = 0.7** is a balanced setting that supports creative yet accurate answers.
- **`max_new_tokens=256`** ensures long enough replies for explanation without overwhelming users.

#### **Anticipated Impact**
- Promotes user-friendly and consistent tone
- Helps reduce hallucinated or off-topic answers
- Makes the assistant behave predictably across varied queries

#### **Iteration & Refinement**
- Initially tested with plain user inputs → added structured `"User:"` and `"Assistant:"` format
- Adjusted temperature from 1.0 to 0.7 for more focused, professional responses

---
## 🧪 User Reviews and Feedback Analysis

### **Methodology**
- Collected feedback via Google Forms and direct peer testing
- Users tested the assistant through the hosted Gradio interface on Hugging Face Spaces

### **Review Collection**

https://docs.google.com/spreadsheets/d/1X_WP3CP08C5zeMPniW8aP2YsPfNQcXEcwQ_mgnj4DMk/edit?usp=sharing

### **Summary of Key Findings**
**Strengths**:
- Natural, clear, and structured replies
- Great for awareness-level information
- Consistent tone and helpful language

**Weaknesses**:
- No spell correction or clarification prompts
- Sometimes gives general answers
- Lacks visual/linked resources

### **Quantitative Metrics**
- **Average Satisfaction Score**: 4.4 / 5
- **Repeat Use Intent**: 8/10 said they would use again

### **Insights Gained**
- Users appreciate **clarity** and **tone**
- Minor spelling issues confuse the assistant
- Users want **more examples or follow-up prompts**

### **Actionable Takeaways**
1. Add **input correction or suggestions** for unclear inputs
2. Introduce **layered responses** or follow-up prompts
3. Include **examples**, links, or images in replies (future work)
4. Explore **query logging** for continuous improvement

---

## 🔮 Future Roadmap

### **Short-Term Goals (Next 1 Week)**
- Add prompt engineering rules to improve fallback responses
- Introduce basic spell-check and re-prompt mechanism
- Polish Gradio UI with helper tooltips or FAQs

### **Mid-Term Goals (2-4 Weeks)**
- Add multilingual support (start with Hindi/Telugu)
- Build context retention between multi-turn queries
- Add cybersecurity FAQs module (static + dynamic)

### **Long-Term Vision (Beyond 4 Weeks)**
- Become a **go-to educational bot** for cybersecurity in schools
- Enable voice-based interaction for visually impaired users
- Collaborate with NGOs or educational orgs for broader deployment

---

## 🚀 Plan to Increase User Adoption

### **Initial User Acquisition**
- Share via LinkedIn, Twitter, and student groups
- Demo in tech clubs, workshops, and Viswam.ai events

### **Value Proposition Communication**
- “Your friendly cybersecurity buddy”
- Quick, understandable, real-time guidance on digital safety

### **Marketing & Promotion**
- Create short demo reels on Instagram and YouTube Shorts
- Write blog posts (Medium/HF Spaces) on building the assistant
- Collaborate with other Hugging Face projects to co-promote

### **Feedback Loops for Continuous Improvement**
- Embed a feedback form after every query/session
- Log user queries (anonymized) to improve training data

### **Community Engagement**
- Publish on GitHub under Apache 2.0 license
- Invite contributors for language support and domain expansions
- Host monthly “Bug Bash + Feature Fest” sprints

---

## 📎 Appendix

**Files**:
- `app.py`: Code for launching Gradio chatbot with TinyLlama
- `requirements.txt`: Minimal dependencies
- `README.md`: Hugging Face deployment metadata

# License 
apache 2.0  by Pooja Kumari  