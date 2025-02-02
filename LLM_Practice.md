# League of Legends LLM Analysis

## Introduction
League of Legends is a popular multiplayer online battle arena (MOBA) game with a competitive scene that draws millions of viewers. Understanding gameplay at a detailed level can be challenging, especially for players looking to improve their skills. This project aims to simplify this process by leveraging a language model to analyze and summarize gameplay from YouTube videos.

## Project Overview
The system provides users with a detailed summary of a League of Legends game. By inputting a YouTube video URL, users receive a breakdown of key moments, highlights, and suggestions for improvement based on the match content.

### Key Features:
1. **YouTube API Integration**: Automatically retrieves the transcript of a given YouTube video.
2. **GPT-4 Integration**: Uses an advanced language model to generate insightful summaries and actionable feedback.
3. **User-Friendly Interface**: A simple input field for users to provide the YouTube URL, with immediate summarized output.

---

## Workflow

### 1. Input URL
The user inputs the URL of a League of Legends gameplay video.

### 2. URL Processing
- **Clean the URL**: Extract the video ID from the provided URL.
- **Verify Validity**: Ensure the video is accessible and contains a transcript.

### 3. Transcript Retrieval
- Utilize the YouTube API to fetch the video transcript.
- Handle errors such as missing or unavailable transcripts.

### 4. Summarization
- Feed the retrieved transcript into GPT-4 with a well-defined prompt.
- The prompt guides the language model to:
  - Highlight key gameplay moments.
  - Identify areas for improvement.
  - Provide a concise summary tailored to League of Legends.

### 5. Output Summary
- The system generates a clean, detailed summary that the user can immediately view.


## Technical Implementation
### Languages and Tools Used:
- **Python**: Backend development and API handling.
- **YouTube API**: Transcript retrieval.
- **OpenAI GPT-4 API**: Language model integration.
- **Gradio**: Simple and interactive web interface for user interaction.

### Challenges and Solutions:
- **Unavailable Transcripts**: Implemented fallback mechanisms to inform users when a transcript is missing.
- **Prompt Tuning**: Iterated on prompts to ensure concise and relevant output from GPT-4.

---

## Future Improvements
1. **Additional Insights**: Incorporate more detailed gameplay metrics such as gold leads, objective control, and team compositions.
2. **Multi-Language Support**: Extend the system to handle videos in languages other than English.
3. **Data Visualization**: Provide graphical representations of gameplay insights.

---

## Conclusion
This project simplifies the process of analyzing League of Legends gameplay, empowering players with actionable insights directly from their chosen videos. By combining YouTube transcript data with the analytical capabilities of GPT-4, this tool represents a significant step toward enhancing strategic understanding and skill development in the game.

---

## How to Use
1. Open the Gradio interface.
2. Input the YouTube URL of a League of Legends gameplay video.
3. Click submit.
4. Receive your tailored game analysis and improvement suggestions within seconds.

