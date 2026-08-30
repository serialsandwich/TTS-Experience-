# The Telephone Society (TTS) - Core Engine

Zero-PII venue session verification engine and touch-hold telemetry processor.

## Repository Structure

* **`verification_engine.py`**: Core verification logic for venue session check-ins, touch telemetry analysis (spatial jitter, pressure variance, micro-timing intervals), and automated account pause triggers.
* **`README.md`**: Technical overview and setup notes.

## Key Principles

* **Zero-PII Privacy**: Verification relies on telemetry variance and cryptographically masked identifiers without storing personal user data.
* **Automated Security**: Non-human input profiles (bots, emulators, fixed-coordinate taps) trigger instant account pause states to maintain system integrity.
