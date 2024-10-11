# LangChain: Summarize Text from YT or Website

This app is designed to streamline the process of summarizing textual content from YouTube videos or websites. It integrates LangChain with the Groq API for natural language processing (NLP) tasks, providing users with concise summaries of various content sources.

## Problem Statement

Extracting key information from long videos or extensive web articles can be time-consuming and overwhelming. People often need quick, digestible summaries of these resources for research, decision-making, or general information gathering. This tool addresses the need for an automated solution that efficiently summarizes large content from YouTube or websites.

## Use Cases

- **Content Creators**: Summarize videos or articles for creating summaries or descriptions.
- **Students/Researchers**: Quickly get the gist of a long video lecture or web article without spending hours watching or reading.
- **Marketers/Content Analysts**: Gain insights from long-form content such as webinars, tutorials, or news articles to make informed decisions.
- **General Users**: Summarize news articles or online resources for quicker consumption.

## Methodology

1. **Input**: Users enter a valid YouTube video URL or website URL, along with their Groq API key.
2. **Validation**: The app checks if a valid API key and URL are provided. It ensures the URL is either a YouTube video or a website URL.
3. **Content Loading**: Based on the input type, the app loads the data using LangChain's `YoutubeLoader` (for YouTube URLs) or `UnstructuredURLLoader` (for websites).
4. **Summarization Chain**: The loaded content is passed through a summarization chain that utilizes a prompt template to generate a summary in 300 words using the Groq API's "Gemma-7b-It" model.
5. **Output**: The summarized content is displayed in the app interface.

## Tech Stack

- **Streamlit**: For creating the web app interface.
- **LangChain**: A framework for building applications powered by large language models.
- **Groq API (Gemma Model)**: To process and summarize the textual content.
- **Python Libraries**: 
  - `validators`: For URL validation.
  - `langchain.prompts`: For creating the prompt templates.
  - `YoutubeLoader`, `UnstructuredURLLoader`: For loading content from YouTube videos or websites.

## Output

The app produces a concise summary of up to 300 words, extracted from the provided YouTube video or web article. The output is presented in a user-friendly format, allowing users to quickly understand the essence of the content.

## Conclusion

This Streamlit app simplifies the process of summarizing content from long YouTube videos and websites using LangChain and the Groq API. By automating the summarization process, it saves users time and effort while providing high-quality summaries for diverse use cases.




# URL Wesbite Eg: https://python.langchain.com/v0.2/docs/introduction/
![{8C3C2219-3A4C-41FD-B819-111221BCC800}](https://github.com/user-attachments/assets/3b001182-ecc3-4eb8-bbb3-fbaa88d9e502)

# YT video Eg: https://www.youtube.com/watch?v=JpHXxsVEVXQ
![{65D3CA69-620D-42E8-862B-705ECAFC8A7E}](https://github.com/user-attachments/assets/2e463b64-d5a0-4b84-8f2b-2500e4703db4)

