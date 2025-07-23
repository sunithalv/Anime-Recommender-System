# Anime Recommender

LLM based application for recommending anime titles based on user preferences. Built with Python, Streamlit, and supports deployment via Docker.

## Features

- Interactive web UI for anime recommendations
- Uses curated anime datasets with genres and synopses
- Modular pipeline for data loading and processing
- Custom exception handling and logging
- Easily extensible and configurable

## Project Structure   

```
.
├── app/                # Streamlit app source
├── config/             # Configuration files
├── data/               # Anime datasets (CSV)
├── pipeline/           # Data processing pipeline
├── src/                # Core logic and utilities
├── utils/              # Custom exceptions, logging
├── chroma_db/          # Vector store/database
├── Dockerfile          # Docker build instructions
├── requirements.txt    # Python dependencies
├── setup.py            # Package setup
```

## Getting Started

### Prerequisites

- [Docker](https://www.docker.com/get-started) installed

### Build and Run with Docker

1. **Build the Docker image:**
   ```sh
   docker build -t anime-recommender .
   ```

2. **Run the container:**
   ```sh
   docker run -p 8501:8501 anime-recommender
   ```

3. **Access the app:**
   Open [http://localhost:8501](http://localhost:8501) in your browser.

### Local Development

1. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

2. Run the app:
   ```sh
   streamlit run app/app.py
   ```

## Configuration

- Edit `config/config.py` for application settings.
- Place your anime datasets in the `data/` directory.

## License

MIT License

---

