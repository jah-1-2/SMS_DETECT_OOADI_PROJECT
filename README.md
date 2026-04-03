# SMS_DETECT_OOADI_PROJECT
Smart Anti-Scam Messaging & Link Detection System
An intelligent Android application designed to protect users from SMS scams, phishing links, and social engineering attacks in real-time. Built with Java for the Android front-end and Python (FastAPI) for the AI-powered backend, the system intercepts incoming messages before the user interacts with them and classifies them as Normal, Suspicious, or Scam.
The app works by listening to incoming SMS messages and app notifications (WhatsApp, Gmail, etc.) the moment they arrive on the device. Each message is parsed, the sender is validated against a trusted database of official short codes (MTN, Orange, banks), and all embedded links are extracted and analyzed. This data is sent to a Python FastAPI backend where an AI model performs deep content analysis — detecting urgency language, impersonation attempts, prize scams, phishing URLs, and PIN requests.
The system is smart enough to distinguish between a friend saying "yo bro hafa" and a scammer pretending to be MTN. It understands youth slang, pidgin, Camfranglais, and informal writing styles. Registered contacts are automatically trusted regardless of message frequency. Unknown senders are subjected to full analysis including a frequency tracker that flags repeated messages within short time windows.
When a threat is detected, the user receives an instant push notification with the risk level and reason — before they even open the message.
Tech Stack: Java · Android SDK · Python · FastAPI · OpenAI API · SQLite · REST API
Target Platform: Android
Status: In Development
