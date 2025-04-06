# Create and activate virtual environment
web: python3.10 -m venv venv
web: source venv/bin/activate

# Install required system-level dependencies
web: sudo apt-get update && sudo apt-get install -y portaudio19-dev python3-dev build-essential libasound2-dev

# Install Python dependencies
web: pip install -r requirements.txt
web: pip install accelerate

# Install PyAudio and simpleaudio (optional, to ensure installation is successful)
web: pip install pyaudio simpleaudio

# Start the application
web: python3 app.py
