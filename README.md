# Chatbot
This code creates a chatbot application using Gradio and OpenAI's GPT-3.5 to create a "sports expert" chatbot named sportspedia.
## How it works
### API Key Setup
- We need to provide our OpenAI API key for accessing GPT models.
### System Message
- The system message {"role": "system", "content": "sports expert"} sets the context that the bot will act as a sports expert.
#### CustomChatGPT Function
- This function handles the user input and sends it to OpenAI’s ChatCompletion.create() method for generating a response.
- It updates the messages list with both user and assistant messages.
- The assistant's response is returned as the output.
### Gradio Interface 
- The gr.Interface() function sets up the user interface, where the user inputs text, and the response from the assistant is displayed as text.
### Sharing
demo.launch(share=True) will allow you to share the Gradio interface publicly.
