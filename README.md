
# Toxic Comment Detector

The Toxic Comment Detector leverages Hugging Face’s **unitary/toxic-bert** model to identify harmful, offensive, or abusive language in user-generated content. Built with a **ReactJS (Vite)** frontend and a **Flask** backend, this tool provides real-time toxicity analysis for enhancing online safety and moderation.

---

## Features

- **Toxicity Detection**: Classifies user-provided text as "Toxic" or "Non-Toxic".
- **Detailed Insights**: Provides confidence scores for specific toxic traits like hate speech or profanity.
- **Real-Time Feedback**: Processes and returns results instantly through an intuitive interface.
- **Open-Source and Customizable**: Easily extendable for additional features or use cases.

---

## Tech Stack

### **Frontend**
- ReactJS with Vite for a fast and responsive UI.
- Axios for API communication.

### **Backend**
- Flask for handling API requests and processing text.
- Hugging Face’s **unitary/toxic-bert** for toxicity detection.

---

## Installation and Setup

### 1. Clone the Repository
```bash
git clone git@github.com:allanninal/toxic-comment-detector.git
cd toxic-comment-detector
```

### 2. Backend Setup
1. Create and activate a virtual environment:
   ```bash
   python3.12 -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate     # Windows
   ```

2. Install dependencies using `requirements.txt` from the backend folder:
   ```bash
   pip install -r backend/requirements.txt
   ```

3. Run the Flask backend:
   ```bash
   python backend/app.py
   ```

### 3. Frontend Setup
1. Navigate to the `frontend` directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the React development server:
   ```bash
   npm run dev
   ```

Visit the app at `http://localhost:5173`.

---

## How It Works

1. **Input Text**: Enter a comment or text to analyze for toxicity.
2. **Backend Processing**: Flask processes the input text using Hugging Face’s `unitary/toxic-bert` model.
3. **Display Results**: The frontend shows the toxicity classification and confidence scores in real-time.

---

## Future Enhancements

1. **Multi-Language Support**: Integrate multilingual models like `xlm-roberta-large` to analyze non-English text.
2. **Custom Toxicity Categories**: Allow fine-tuning models for user-defined toxicity classifications.
3. **Explainability**: Provide detailed insights into why a comment is classified as toxic.
4. **Live Moderation**: Integrate real-time toxicity detection with chat systems for instant moderation.

---

## Alternatives for Toxic Comment Detection

1. **cardiffnlp/twitter-roberta-base-offensive**: Best for social media applications like Twitter.
2. **facebook/bart-large-mnli**: Offers zero-shot classification for custom toxicity categories.
3. **Perspective API (Google)**: Provides multi-dimensional toxicity scores for hate speech, threats, and more.
4. **TextBlob with Custom Rules**: A lightweight library for sentiment and basic toxicity analysis.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Support

If you find this project helpful, consider supporting me on Ko-fi:  
[ko-fi.com/allanninal](https://ko-fi.com/allanninal)

---

## Explore More Projects

For more exciting projects, check out my list of **AI Mini Projects**:  
[Mini AI Projects GitHub List](https://github.com/stars/allanninal/lists/mini-ai-projects)
