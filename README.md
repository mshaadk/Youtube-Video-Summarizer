# YouTube Video Summarizer
This project is a web application built using **Streamlit** that allows users to summarize YouTube videos based on their transcripts. It leverages **Google's Gemini Model** to generate concise summaries from the extracted transcripts.

![image](https://github.com/user-attachments/assets/91496b01-455a-495f-a83e-107c24fc78d7)

## Features
- Extracts YouTube video transcripts using the [YouTube Transcript API](https://github.com/jdepoix/youtube-transcript-api).
- Summarizes transcripts into concise bullet points using Google's Gemini Model.
- Provides video thumbnails along with the summary for better visualization.
- Interactive and simple-to-use interface powered by Streamlit.

##  Installation
To run this project locally, follow these steps:

**1. Clone the repository:**

```python
git clone https://github.com/mshaadk/Youtube-Video-Summarizer.git
cd youtube-video-summarizer
```

**2. Create a virtual environment and install dependencies:**

```python
python3 -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

**3. Set up environment variables:**

Create a `.env` file in the root directory and add your Google API key and other configurations:

```python
GOOGLE_API_KEY=your_google_api_key
```

**4. Run the Streamlit app:**

```python
streamlit run app.py
```

## Usage
1. Open the app in your browser.
2. Enter the YouTube video URL you want to summarize.
3. Click on the "Get Summary" button to generate a concise summary.

## Code Overview
`app.py`
- **YouTube Transcript Extraction:** Uses the `YouTubeTranscriptApi` to fetch video transcripts.
- **Summarization:** Passes the transcript to Google's Gemini Model for summarization.
- **Streamlit UI:** Provides a simple UI to input video URLs and display results, including thumbnails and summaries.

`set_bg_from_url()`
- Sets a custom background image for the app.
  
## Example
Enter a YouTube URL and see a sample summary of the video transcript:

```makefile
Input: https://www.youtube.com/watch?v=xyz
Output: Summarized points of the video in under 250 words.
```

## Contributing
Contributions are welcome! Feel free to submit a pull request or raise issues for any bugs or feature requests.

## License
This project is licensed under the [MIT License](LICENSE.txt). See the LICENSE file for more details.
