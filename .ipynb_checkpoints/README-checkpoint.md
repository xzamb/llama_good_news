# Llama Good News 🦙📰

A Python-based news filtering tool that uses AI to extract and summarize only the positive news from websites, helping you stay informed without the negativity.

## 🌟 Project Overview

In today's world, news can often be overwhelming and negative. This project aims to create a more positive news consumption experience by:

- **Web Scraping**: Automatically fetching content from news websites
- **AI-Powered Filtering**: Using Llama 3.2 (via Ollama) to intelligently identify and extract only positive news
- **Smart Summarization**: Generating concise summaries that focus exclusively on good news while filtering out harmful or sad content

## 🚀 How It Works

1. **Content Extraction**: The tool scrapes website content using BeautifulSoup, removing irrelevant elements like scripts, images, and styling
2. **AI Processing**: Content is sent to Llama 3.2 with a specialized prompt that instructs it to focus only on positive news
3. **Filtered Output**: The AI returns a summary containing only the good news, filtering out anything that might be harmful or make people sad
4. **Display**: Results are presented in a clean, readable markdown format

## 🛠️ Technical Stack

- **Python**: Core programming language
- **Ollama**: Local AI model management and inference
- **Llama 3.2**: The AI model used for content analysis and summarization
- **BeautifulSoup**: Web scraping and HTML parsing
- **Requests**: HTTP requests for fetching web content
- **Jupyter Notebook**: Interactive development environment

## 📋 Prerequisites

- Python 3.11+
- Ollama installed locally
- Llama 3.2 model downloaded (`ollama pull llama3.2`)

## 🔧 Dependencies

```bash
pip install requests ollama python-dotenv beautifulsoup4 ipython
```

## 💡 Usage

Simply run the Jupyter notebook (`main.ipynb`) and call the `get_summary()` function with any news website URL:

```python
get_summary("https://your-news-website.com")
```

The tool will automatically:
- Fetch the website content
- Process it through the AI model
- Display only the positive news in a formatted summary

FYI: It only works with non-js websites for now.

## 🎯 Key Features

- **Positive Focus**: Specifically designed to filter out negative news
- **Local AI**: Uses Ollama for privacy-focused, local AI processing
- **Flexible**: Can work with any news website
- **Clean Output**: Presents results in readable markdown format
- **Customizable**: Easy to modify the AI model or adjust filtering criteria

## 🔄 Example Workflow

1. The tool visits a news website (e.g., globo.com)
2. Scrapes and cleans the content
3. Sends it to Llama 3.2 with instructions to extract only good news
4. Receives a filtered summary focusing on positive stories
5. Displays the results in an easy-to-read format

## 🤖 AI Prompt Strategy

The system uses a carefully crafted prompt that instructs the AI to:
- Act as a "brilliant summarizer" focused on good news
- Remove any bad news (defined as anything harmful or that might make people sad)
- Emphasize the importance of focusing only on positive content

## 🌍 Purpose

This project addresses the common problem of news fatigue and negativity bias in media consumption. By automatically filtering for positive news, it helps users stay informed about good things happening in the world without being overwhelmed by negative content.

---

*Stay positive, stay informed!*
