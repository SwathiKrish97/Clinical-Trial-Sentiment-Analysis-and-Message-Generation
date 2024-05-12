# Clinical Trial Sentiment Analysis and Message Generation

## Project Overview
This project aims to scrape Reddit posts and comments from the subreddit related to epilepsy, perform sentiment analysis on the text, and generate personalized messages using the OpenAI API. The goal is to engage users who express interest in or could benefit from participating in clinical trials.

## Setup Instructions

### Prerequisites
- Python 3.x
- `praw`, `transformers`, `torch`, and `openai` libraries
- OpenAI and Hugging Face API keys
- Reddit API credentials (client_id, client_secret, user_agent)

### Installation
1. Install the necessary Python packages:
!pip install openai==0.28 transformers torch praw

2. Ensure that the environment variables for OpenAI API key (`OPENAI_API_KEY`) and Hugging Face token (`HF_TOKEN`) are set correctly.

### Running the Code
Run the script in a Python environment (e.g., Jupyter notebook, Python script). Ensure all API keys and environment variables are set correctly before execution.

Follow these steps to run the Jupyter notebook associated with this project:

1. **Open the Terminal**:
   - For Windows, search for and open 'Command Prompt'.
   - For macOS, search for and open 'Terminal'.

2. **Navigate to the Project Directory**:
   - Change to the directory where your project is located using the `cd` command:
     ```bash
     cd path_to_your_project_directory
     ```

3. **Start Jupyter Notebook**:
   - Launch Jupyter Notebook by running:
     ```bash
     jupyter notebook
     ```
   - This command will open Jupyter in your default web browser.

4. **Open the Notebook File**:
   - In the Jupyter Notebook interface, navigate to and click on the `.ipynb` file to open it.

5. **Run the Notebook Cells**:
   - Execute the code in each cell sequentially by selecting the cell and pressing `Shift + Enter`, or by using the 'Run' button in the toolbar.

6. **Save and Exit**:
   - Save your work by clicking `File` > `Save`, or press `Ctrl + S` (`Cmd + S` on macOS).
   - To exit, close the browser tabs/windows and stop Jupyter in your terminal by pressing `Ctrl + C`.

These instructions will guide you through opening, running, and interacting with the Jupyter notebook for this project.

## Methodology
- **Data Collection:** Using `praw`, the Python Reddit API Wrapper, to scrape comments from the subreddit 'Epilepsy'.
- **Sentiment Analysis:** Utilizing `transformers` and `torch` with the `bert-base-multilingual-uncased-sentiment` model to predict sentiment scores from comments.
- **Message Generation:** Using the OpenAI API to generate personalized messages based on the sentiment scores of the comments.

## Challenges Faced
- Handling API rate limits and ensuring efficient API calls.
- Ensuring accuracy in sentiment prediction across different contexts within the comments.
- Generating relevant and engaging responses through the OpenAI API based on varied sentiments.

## Ethical Considerations
- Ensured compliance with Reddit's API terms of use to respect user privacy and data use policies.
- Applied sentiment analysis and AI-generated messaging responsibly to avoid generating inappropriate or sensitive content.

## Examples
- Collected data includes comments from Reddit users discussing their experiences with epilepsy.
- Analyzed sentiments ranged from "very negative" to "very positive".
- Generated messages aimed to provide support, information, or engagement based on the user's sentiment and content of the comment.

## Conclusion
This project demonstrates the use of modern AI tools for sentiment analysis and automated message generation, aiming to enhance user engagement and provide insights into public sentiment on clinical trials in the medical community.



