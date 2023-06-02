# SmartTalk Bot Assistant
A chatbot assistant built using LangChain and powered by the LLM.

SmartTalk is an advanced conversational application built using the LangChain framework and LLMs (Large Language Models). It leverages OpenAI's GPT-3.5 generation models to provide a range of features including chatbot-style question-answering, generative question-answering, summarization, and more. The application is designed to be extensible and customizable by "chaining" together different components.

## Key Features

- Chatbot-style question-answering: SmartTalk can provide responses to various questions using pre-defined chatbot-style prompt templates.
- Generative Question-Answering (GQA): It can generate detailed answers to questions by utilizing the power of LLMs.
- Summarization: SmartTalk is capable of generating summaries of given text inputs.
- Integration with external tools: It can utilize tools like Google Search and OpenWeatherMap to enhance its functionality.

## Installation

1. Obtain an OpenAI API key: To use SmartTalk, you need to have an OpenAI API key. If you don't have one, you can sign up for OpenAI and obtain the API key from your account.

2. Set up environment variables: After obtaining the API key, you need to set it as the value of the `OPENAI_API_TOKEN` environment variable. In Python, you can do this by adding the following line of code:

   ```python
   import os
   os.environ['OPENAI_API_TOKEN'] = 'YOUR_OPENAI_API_KEY'

3. Install the required dependencies: SmartTalk relies on the openai library. You can install it using pip:
----------------------
#### pip install openai
----------------------

4. Set up additional environment variables: Depending on the specific functionality you want to use, SmartTalk requires certain environment variables to be set. These include:

* __GOOGLE_CSE_ID:__ Google Custom Search Engine (CSE) ID for integrating Google Search functionality.
* __GOOGLE_API_KEY:__ API key for Google Search integration.
* __OPENWEATHERMAP_API_KEY:__ API key for OpenWeatherMap integration.

5. Clone the SmartTalk repository: Clone the SmartTalk repository from GitHub to your local machine.
---------------------
#### git clone https://github.com/your-username/smarttalk.git
---------------------

6. Start using SmartTalk: You can now import the necessary modules from the SmartTalk library and start using its features in your Python code.

## Usage

To use SmartTalk, follow these steps:

1. Initialize the necessary components: Create an instance of the OpenAI LLM, load the required tools (e.g., Google Search, OpenWeatherMap), and set up any additional configurations.
2. Set up the prompt and memory: Define the prompt template to be used by the ZeroShotAgent, which combines the LLM and tools. Optionally, configure a conversation buffer memory to store and retrieve conversation history.
3. Create the agent: Instantiate a ZeroShotAgent using the LLMChain and tools, specifying any additional options or configurations.
4. Execute queries: Use the AgentExecutor to run queries and interact with the SmartTalk application. Provide the input query or question, and the agent will generate a response using the configured LLM and tools.
5. Repeat as needed: You can continue to interact with SmartTalk by running additional queries through the AgentExecutor.

## Contributing
Contributions to SmartTalk are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the GitHub repository.

## License
This project is licensed under the MIT License.
