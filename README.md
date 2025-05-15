# YouTube Comments Sentiment & Engagement Analysis

Welcome to the **YouTube Comments Sentiment & Engagement Analysis** project — a comprehensive Python pipeline that extracts, analyzes, and visualizes YouTube video comments to provide actionable insights into viewer sentiment and engagement dynamics.

---

## 🚀 Project Overview

This tool leverages the YouTube Data API to fetch comments from any public video and combines advanced natural language processing (NLP), sentiment analysis, and emoji parsing to paint a vivid picture of audience reactions. Beyond simple counts, it calculates a **custom engagement score** that balances quantitative metrics (likes, views, subscribers) with qualitative insights (sentiment polarity, emoji sentiment, comment length) — a holistic metric designed for content creators, marketers, and data scientists alike.

---

## 🔍 Key Features

* **YouTube Video Metadata Extraction:** Automatically pulls video title, channel info, view count, likes, comments, and subscriber count.
* **Bulk Comment Download:** Fetches all available top-level comments using efficient pagination.
* **Sentiment Classification:** Classifies comments into positive, neutral, or negative using TextBlob’s polarity analysis.
* **Emoji Sentiment Detection:** Parses and quantifies emoji-based emotional signals embedded in comments.
* **Named Entity Recognition:** Identifies mentions of people in comments leveraging spaCy’s NLP pipeline.
* **Word Clouds:** Visualizes frequent terms for positive and negative comment clusters.
* **Custom Engagement Score:** A multi-factor, normalized metric incorporating sentiment, emoji impact, subscriber scale, and comment quality.
* **CSV Export:** Easily export analyzed data for further exploration or reporting.

---

## 📈 Engagement Score — A Next-Level Metric

Traditional engagement metrics often overlook the nuanced emotional tone and qualitative depth of audience interaction. This project’s engagement score innovates by integrating:

* Positive comment ratio weighted by sentiment polarity.
* Emoji sentiment intensity.
* Comment length and likes per comment as proxies for comment quality.
* Normalized subscriber interaction using logarithmic scaling.
* Classic metrics like likes-to-views and comments-to-views ratios.

The result? A rich, dynamic measure of audience engagement that captures both volume and vibe.

---

## 🛠️ Technologies Used

* Python 3.x
* Google API Client for YouTube Data API v3
* TextBlob for sentiment analysis
* spaCy for Named Entity Recognition
* emoji for emoji parsing
* WordCloud and Matplotlib for visualization
* Pandas and NumPy for data manipulation
* Seaborn for enhanced plotting aesthetics
* tqdm for progress bars

---

## 🔧 Setup Instructions

1. Clone this repository:

   ```
   git clone https://github.com/your-username/youtube-comments-analysis.git
   ```
2. Install required packages:

   ```
   pip install -r requirements.txt
   ```
3. Obtain a YouTube Data API key from the [Google Developer Console](https://console.developers.google.com/).
4. Update `API_KEY` in the script with your key.
5. Run the script and input the YouTube video URL when prompted.

---

## 📊 Usage & Output

* The script outputs summary statistics on video metadata and comment sentiment.
* Generates sentiment distribution plots and word clouds.
* Calculates and displays a custom engagement score.
* Saves a CSV file of detailed comment-level analysis for offline use.

