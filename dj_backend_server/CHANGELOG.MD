2.18.2024
- The conversational retrieval functionality is now operating as expected. It successfully sends the conversation history to the language model, allowing the context from previous interactions to be utilized effectively.
- Added support for Ollama as the Language Model (LLM). Ensure Ollama is specified in the .env configuration and the model is preloaded on the server.

2.17.2024
- Incorporate 'Ollama' into your example.env configuration and make sure to reflect these changes in your .env file for compatibility.
- We've expanded the logging capabilities within settings.py by deploying logging.debug for more detailed insights, although it remains inactive when the DEBUG mode is off.
- We've refreshed the dependencies listed in requirements.txt to ensure the latest support and functionality.
- Updates to LangChain and OpenAI libraries, now feature the exciting addition of Ollama, currently under development. 
- This version has a significant update that is still pending comprehensive testing; therefore, we advise against deploying it in production environments until it is fully vetted.
- Modifications have been made to the history module to append the input message to requests sent to OpenAI. These changes are still being tested. (disabled for the moemnt)

2.14.2024
- Added example.env to streamline environment setup.
- Implemented translation fixes to enhance application localization.
- Updated docker-compose.yaml to prefix each container with oc_ for better namespace management.
- Performed fixes in requirements.txt for improved dependency resolution.
- Ensured existence of Vector Database (QDrant) prior to web crawling operations to address issues encountered with large websites, ensuring Vector Database creation and availability.