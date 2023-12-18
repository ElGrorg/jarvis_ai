# jarvis_ai
Conversational AI Program similar to Jarvis from MCU

**Developed By: Greg Salmon**

## Installation
1. Download the zip file
2. Install necessary packages using the terminal command `pip install -r requirements.txt`
3. In terminal, Create a `.env` file using the command `touch .env`
    - Inside the `.env` file, type:
    `OPENAI_API_KEY="Your Key Here"`
## Running the Program
This program will run continuously until ended
Run the command `sudo python3 jarvis.py`
    - Important to note: We use the `sudo` attribute because the program utilizes the keyboard library, which essentially allows the program to view keystrokes. 
    - When you first run the program, it may fail and prompt you to update your computer accessibility settings.
    - You may also be prompted to allow microphone access
    - There is no malicious code to worry about but I recommend always previewing the code prior to running it on your computer if you are concerned

- To record your message to Jarvis, press **"esc"** when prompted
- To end your recording, press **"esc"** again
- Jarvis will provide a response within 15 seconds, delay depends on length of question and memory
- To quit the program, press **"ctrl+C"**
- Message history is stored in the `/conversation_history/` directory
    - To view an example message history, see `/conversation_history/example_message/example_message.csv`

## Comments
- This program currently runs via the openai API, which costs money.
    - Applications used include Whisper, Chat Generation, and Text to Speech
- **BE WARNED**, while it is inexpensive, accidentally leaving the recording running will cause the openai billing to significantly increase, as the audio models cost the most

## Final Thoughts
I originally developed this program with open source tools found on HuggingFace. I decided to transition to openai due to its speed. My previous iteration took around 30-45 seconds per response, which is not acceptable for a real time chatbot. 

### Future plans include:
- Moving towards all open-source/free models
- Cleaning code
- Decrease time to response
