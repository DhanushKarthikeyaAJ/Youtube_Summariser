
# YouTube Video Summarizer

## Project Description

The YouTube Video Summarizer is a mini NLP project designed to provide concise summaries of YouTube videos based on their subtitles. By leveraging advanced natural language processing (NLP) techniques and transformer models like BART, DistilBART, BERT, and GPT-2, this tool extracts the key points from video subtitles to give users a quick understanding of the video content. This is especially useful for educational or lengthy videos, allowing users to save time by reading a short summary before deciding to watch the full video.

## Features

- Extractive summarization of YouTube video subtitles.
- Uses transformer-based models (e.g., BART, DistilBART) for generating summaries.
- Suitable for videos with subtitles, providing accurate and concise information.
- Helps in quickly grasping the main content of lecture videos or tutorials.

## Installation

To run this project locally, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/youtube-summarizer.git
   cd youtube-summarizer
   ```

2. **Create a virtual environment (optional but recommended):**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. **Install the required dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

   *(Make sure to create a `requirements.txt` file with all the dependencies like `transformers`, `torch`, `numpy`, etc.)*

## Usage

1. **Run the summarizer script:**

   Use the provided script to summarize a YouTube video based on its subtitles:

   ```bash
   python summarize_youtube.py --url "https://www.youtube.com/watch?v=example" --model "bart"
   ```

   Replace `--url` with the link to the YouTube video you want to summarize and choose the model type with `--model` (options: `bart`, `distilbart`, `bert`, `gpt-2`).

2. **Sample Output:**

   After running the script, you'll get a brief summary of the video content in the terminal. This summary will highlight the key points covered in the video, making it easier to decide whether to watch the full video.

## Example

Here's an example of how you might use the YouTube summarizer:

```bash
python summarize_youtube.py --url "https://www.youtube.com/watch?v=example_video_id" --model "bart"
```

Output:

```
Summary: This video covers the basics of machine learning, including supervised and unsupervised learning techniques. Key algorithms like linear regression and k-means clustering are explained with examples.
```

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgments

- [Hugging Face Transformers](https://huggingface.co/transformers/)
- [YouTube API](https://developers.google.com/youtube/)
- [Analytics Vidhya Blog on YouTube Summariser](https://www.analyticsvidhya.com/blog/2022/01/youtube-summariser-mini-nlp-project/)
