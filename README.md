# EntertainmentBot

EntertainmentBot is an interactive chatbot that recommends entertainment options and engages users with fun content. It provides personalized recommendations for movies, TV series, music, games, and books based on user preferences.

## Features

- Greets users and asks for their entertainment preferences
- Provides recommendations based on user input
- Offers trivia, jokes, and stories throughout the conversation
- Generates a JSON summary of user preferences and recommendations

## Prerequisites

Before running the EntertainmentBot, make sure you have the following installed:

- Python 3.7 or higher
- pip (Python package installer)

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/EntertainmentBot.git
   cd EntertainmentBot
   ```

2. Install the required libraries:
   ```
   pip install openai 
   ```
   ```
   pip install python-dotenv
   ```

## OpenAI API Key

To use the OpenAI API, you need to obtain an API key:

1. Sign up for an account at [OpenAI](https://openai.com/)
2. Navigate to the API section and create a new API key
3. Create a `.env` file in the project root directory
4. Add your API key to the `.env` file:
   ```
   OPENAI_API_KEY=your_api_key_here
   ```

## Usage

1. Run the Jupyter Notebook:
   ```
   jupyter notebook EntertainmentBot.ipynb
   ```

2. Execute all cells in the notebook

3. Interact with the EntertainmentBot using the chat interface

## How it Works

1. **API Setup**: The code uses the OpenAI API to generate responses. It loads the API key from the `.env` file using the `dotenv` library.

2. **Helper Functions**: 
   - `get_completion()`: Sends a single prompt to the OpenAI API
   - `get_completion_from_messages()`: Sends a list of messages to the OpenAI API

3. **Chat Interface**: The `collect_messages()` function handles user input and bot responses. It uses the Panel library to create an interactive chat interface.

4. **Context and Knowledge Base**: The bot's knowledge and behavior are defined in the `context` variable. This includes information about various entertainment genres and options.

5. **User Interaction**: 
   - The bot greets the user and asks for their preferences
   - Based on user input, it recommends entertainment options
   - It can provide trivia, jokes, and stories to keep the conversation engaging

6. **JSON Summary**: After the conversation, the bot can generate a JSON summary of the user's preferences and recommendations.

## Customization

You can customize the bot's knowledge base by modifying the `context` variable in the notebook. This allows you to add or change entertainment options, genres, and other information the bot can provide.

## License

[MIT License](LICENSE)

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Acknowledgments

- OpenAI for providing the GPT model
