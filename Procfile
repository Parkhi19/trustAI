# Create and activate virtual environment
web: python3.10 -m venv venv
web: source venv/bin/activate

# Install required Python dependencies
web: pip install -r requirements.txt
web: pip install accelerate

# Install system-level dependencies (should be managed via Docker or buildpack, but you can include them here as a fallback)
web: sudo apt-get update && sudo apt-get install -y portaudio19-dev python3-dev build-essential

# Install Python-specific dependencies
web: pip install portaudio

# Start your application
web: python3 app.py


