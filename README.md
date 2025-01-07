# Whatsapp-AI-chatbot-using-LLM
This project demonstrates a WhatsApp AI chatbot powered by a Large Language Model (LLM) integrated with Twilio’s API. The chatbot can process incoming messages, generate intelligent responses, and send replies directly through WhatsApp.


# Key Features:
LLM-Powered Responses – Uses a language model to dynamically generate responses to user queries.
Twilio WhatsApp Integration – Leverages Twilio’s API for seamless message exchange on WhatsApp.
FastAPI Backend – Built with FastAPI to handle incoming requests and manage responses efficiently.
CTransformers Integration – Uses CTransformers to load and run the LLM model (OpenHermes-2 Mistral 7B).
Logging and Error Handling – Implements logging to track message delivery and handle errors gracefully.

# Technologies Used:
Python
FastAPI
Twilio API
LangChain
CTransformers
dotenv (for managing environment variables)

# Setup Instructions:
1 Clone the repository.

2 Install dependencies:

!pip install fastapi twilio langchain CTransformers python-dotenv


# Set up your .env file with:

TWILIO_ACCOUNT_SID = "your_account_sid"  
TWILIO_AUTH_TOKEN = "your_auth_token"  
TWILIO_NUMBER = "your_twilio_number"  
 
# Run the FastAPI app:

uvicorn twilio_app:app --reload

# How It Works:
Users send a message via WhatsApp.
The chatbot receives the message and sends it to the LLM.
The LLM generates a response, which is then relayed back to the user through Twilio’s WhatsApp API.
