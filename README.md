Smart Health Assistant - README

Overview
The Smart Health Assistant is a Flask-based web application that provides general health advice and information about common symptoms. It uses Cohere's AI for generating responses and gTTS (Google Text-to-Speech) for audio output.

Features
- Conversational AI interface for health-related queries
- Voice input capability (browser speech recognition)
- Text-to-speech output for responses
- Conversation logging
- Health knowledge base for common symptoms
- Responsive web interface

Installation

1. Clone the repository:
   ```bash
   git clone [repository-url]
   cd [repository-name]
 

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
 

3. Set up environment:
   - Create a `.env` file with your Cohere API key:
     
     COHERE_API_KEY=your_api_key_here
   

Running the Application

Start the Flask development server:
```bash
python app.py


The application will be available at `http://localhost:5000`

Configuration

- The Cohere API key is currently hardcoded in `app.py` (should be moved to environment variables for production)
- Audio files are stored in the `audio/` directory
- Conversation logs are saved to `conversation_log.txt`

Usage

1. Open the web interface in your browser
2. Type your health-related question in the input field or click the microphone button for voice input
3. Click the send button or press Enter to submit your question
4. Click the speaker icon on responses to hear them read aloud

Health Topics Covered

The assistant can provide information about:
- Common symptoms (headache, fever, nausea, etc.)
- General wellness advice
- Healthy lifestyle recommendations
- When to consult a healthcare professional

Limitations

- Not a substitute for medical advice**: The assistant provides general information only
- No medication recommendations**: Will not suggest specific medications
- Limited to health topics**: Will redirect non-health related questions

Files Structure

- `app.py`: Main Flask application
- `index.html`: Web interface
- `style.css`: Styling for the web interface
- `requirements.txt`: Python dependencies
- `conversation_log.txt`: Log of all conversations
- `audio/`: Directory for generated speech files

License

This project is licensed under the MIT License. See the LICENSE file for details.

Disclaimer

This application is for educational purposes only and does not provide medical advice. Always consult with a qualified healthcare professional for medical concerns.
