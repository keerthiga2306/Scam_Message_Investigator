# Scam Message Investigator

## Project Overview

Scam Message Investigator is an AI-powered web application developed using Python, Streamlit, and Ollama. It helps users identify potential scams in SMS messages, emails, WhatsApp messages, and online offers.

The application uses the Gemma 3:1B language model to analyze messages, detect suspicious indicators, assess risk levels, and provide safety recommendations.

## Features

- **Message Analysis:** Analyzes SMS, emails, WhatsApp messages, and online offers.
- **Risk Detection:** Classifies messages into Low Concern, Medium Concern, and High Concern.
- **Warning Signs:** Identifies suspicious links, urgent language, OTP requests, fake offers, and advance payment requests.
- **Safety Recommendations:** Provides suggestions to avoid potential online scams.
- **Investigation Report:** Displays the analysis in a structured format.
- **Dark Theme UI:** Provides a simple and user-friendly interface.

## Technologies Used

- Python
- Streamlit
- Ollama
- Gemma 3:1B
- JSON
- Requests

## System Requirements

- Python 3.10 or above
- Ollama installed
- Gemma 3:1B model downloaded
- VS Code or any Python IDE

## Installation and Setup

### 1. Clone the Repository

```bash
git clone <your-repository-link>
```

### 2. Navigate to the Project Folder

```bash
cd Scam-Message-Investigator
```

### 3. Install Required Libraries

```bash
pip install streamlit requests
```

### 4. Install and Run Ollama

Download Ollama from:

https://ollama.com/

### 5. Download the Gemma Model

```bash
ollama pull gemma3:1b
```

### 6. Run the Application

```bash
streamlit run app.py
```

The application will open in your web browser.

## How It Works

1. The user enters a suspicious message.
2. Streamlit collects the message.
3. Python sends the message to the Ollama API.
4. The Gemma 3:1B model analyzes the message.
5. The AI returns a structured JSON response.
6. The application displays the risk level, warning signs, summary, and safety recommendations.

## Risk Levels

| Risk Level | Description |
|---|---|
| Low Concern | No clear warning signs identified |
| Medium Concern | Some suspicious indicators detected |
| High Concern | Multiple serious scam indicators detected |

## Example Input

```text
Congratulations! You won ₹50,000.
Click this link and pay ₹500 to claim your prize.
```

## Expected Output

- Risk Level: High Concern
- Message Type: Fake Prize Notification
- Warning Signs: Unrealistic prize offer and advance payment request.
- Recommended Action: Do not click suspicious links or make advance payments. Verify through official channels.

*Note: AI-generated results are assessments, not proof that a message is fraudulent.*

## Future Enhancements

- URL safety checking.
- Email attachment analysis.
- Multi-language message analysis.
- Message history and report downloads.
- Improved scam detection accuracy.

