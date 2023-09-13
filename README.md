# ai-chatbot-RP

Client/User Interface

We will use React to build the user interface. The seller facing Chat UI will communicate with the backend via WebSockets.

We are using GPT-J-6B which is a pre-trained model for this demo but however, in the future, we intend to have our own trained model based on the dataset of the present seller questions and answers.

We are using Redis JSON to store the chat data and also using Redis Streams for handling the real-time communication with the huggingface inference API.

To send messages between the client and server in real-time, we need to open a socket connection. We are using FastAPI for the chat server.
