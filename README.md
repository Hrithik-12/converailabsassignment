# converailabsassignment

# 🚀 Call Quality Analyzer

This project is a **Voice AI system** that analyzes sales call recordings to extract key insights such as speaker talk-time, sentiment, and actionable feedback.  

The system takes a **YouTube call recording URL** as input and returns:  
1. **Talk-time ratio** → % of conversation spoken by each person  
2. **Number of questions asked**  
3. **Longest monologue duration**  
4. **Call sentiment** → Positive / Negative / Neutral  
5. **One actionable insight**  

Bonus: Detect which participant is the **sales rep vs customer**.  

---

## 🔄 System Workflow

diagram : <img width="861" height="886" alt="diagram-export-19-09-2025-17_35_27" src="https://github.com/user-attachments/assets/ed391973-fae4-43da-8661-07728977ab75" />


**Explanation of Flow:**  
- Input: YouTube video URL  
- **Process 1:** Extract audio from the video  
- **Transcription:** Convert speech to text (using Whisper or similar)  
- **Process 2:** Regex-based detection for questions  
- **Process 3:** Split transcript for talk-time ratio + monologue analysis  
- **Process 4 & 5:** Sentiment detection and actionable insight generation  
- **Prompt + AI Model:** Use LLM (e.g., Gemini / GPT) to refine insights  
- **Output:** Structured metrics and insights  

---

## 📂 Assignment Details

- Must work with this [test file](https://www.youtube.com/watch?v=4ostqJD3Psc)  
- Handle **poor audio quality**  
- Processing time **< 30 seconds**  
- Runs on **free Google Colab tier**  
- Code should be **commented** for clarity  

---

## 🧪 Example Approach

- **Transcription:** Extract text from YouTube audio using `yt-dlp` + `Whisper`  
- **Talk-time Ratio:** Separate by speaker markers (`#`) and count words  
- **Questions:** Regex scan for `?`  
- **Sentiment:** Run transcript through Hugging Face sentiment models or LLMs  
- **Monologues:** Measure longest uninterrupted speech segment  
- **Insight:** Prompt AI model to summarize and generate one actionable recommendation  

---

## ▶️ How to Run

1. Open the notebook in Colab:  
   [Colab Notebook](https://colab.research.google.com/drive/1NsRmR1fQouleju5yjSpv1ta---ulp-oP?usp=sharing)

2. Run all cells step by step.  
3. Input the YouTube URL when prompted.  
4. Get results including **talk-time, sentiment, questions, monologue, and insights**.  

---

## 📅 Submission

- Deliverables:  
  1. GitHub repo with Colab notebook  
  2. Short explanation of approach (<200 words)  

---

👩‍💻 Let’s build the future of **Voice AI** together!  

