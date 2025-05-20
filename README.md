# Chatbot-using-RASA
This is a chatbot built using the [Rasa](https://rasa.com/) open-source framework. 
The bot is designed to understand user inputs and respond intelligently based on predefined intents and stories. 

# Features
- Natural Language Understanding (NLU)
- Dialogue Management with stories
- Custom Actions 
- Easy to train and extend

# Project Structure
- nlu.yml – Natural Language Understanding
      This file trains Rasa to recognize intents and 
      entities from user messages.
      * Intent: What the user wants to do (e.g., greet, 
         book_flight)
      *Examples: Sample user messages for that intent
  
- domain.yml – Bot Capabilities
    Defines the intents, entities, slots, responses, 
    actions, and optionally forms.
    * responses: Templates the bot can say (used in 
        utter_* actions)
    *actions: Custom or default actions

- stories.yml – Conversation Paths
    Defines sample conversations that train the dialogue 
    management model.

# Steps to Run Rasa
- Install Prerequisites
    python --version
    pip --version
- Install Rasa
    pip install rasa
- Train the Bot
    rasa train
- Run the Rasa Bot
    rasa shell
- Start the Rasa Server
    rasa run --enable-api --cors "*" --debug




