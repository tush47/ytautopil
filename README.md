# YouTube Automation using Crew AI
This project leverages Crew AI agents and Python libraries to automate the workflow for YouTube channel owners. By utilizing the YouTube API and a free LLM (Language Learning Model), this automation reduces the workload of finding trending video topics.

## Features

- **Crew AI Agents**: Configured using TOML files to streamline tasks.
- **YouTube API**: Accessed via Google Cloud to gather relevant data.
- **Trending Video Topics**: Automated process to find trending topics using a free LLM model.
- **Ease of Use**: Simple commands and setup process to get started quickly.

## Installation

### Prerequisites

- Python 3.7+
- [Poetry](https://python-poetry.org/) for dependency management
- Google Cloud account for accessing the YouTube API

### Steps

1. **Clone the Repository**

    ```sh
    git clone https://github.com/yourusername/youtubeautomation.git
    cd youtubeautomation
    ```

2. **Install Dependencies**

    Use Poetry to install the project dependencies:

    ```sh
    poetry install
    ```

3. **Setup Google Cloud**

    - Create a project on [Google Cloud Platform](https://cloud.google.com/).
    - Enable the YouTube Data API v3.
    - Create credentials (API Key) and download the JSON file.
    - Set the environment variable for the API key:

      ```sh
      export GOOGLE_APPLICATION_CREDENTIALS="path/to/your/credentials.json"
      ```

## Configuration

1. **Crew AI Agents**

    Configure the agents using the `config.toml` file. Here's a sample configuration:

    ```toml
    [agent]
    name = "YouTubeAutomationAgent"
    tasks = ["find_trending_videos"]

    [youtube]
    api_key = "YOUR_YOUTUBE_API_KEY"
    ```

2. **LLM Model**

    Ensure you have access to a free LLM model. This can be integrated within the code to analyze and suggest trending topics.

## Usage

1. **Run the Automation**

    Execute the main script to start the automation process:

    ```sh
    poetry run python main.py
    ```

    The script will use Crew AI agents and the YouTube API to fetch trending video topics and suggest new content ideas.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for review.
---

Happy Automating!
