# Financial Advisor AI

An AI-powered financial advisor built with phidata that provides financial insights and analysis through an interactive playground interface.

## Overview

This project implements two AI agents:
- **Finance Agent**: Analyzes financial data using YFinance tools
- **Web Agent**: Searches the web for additional information using DuckDuckGo

Both agents are powered by Groq's llama-3.3-70b-versatile model and are accessible through a user-friendly web interface.

## Features

- **Stock Price Analysis**: Get real-time stock prices and historical data
- **Analyst Recommendations**: View professional analyst opinions on stocks
- **Company Information**: Access detailed company profiles and metrics
- **Financial News**: Stay updated with the latest company and market news
- **Web Search Integration**: Find additional financial information from across the web
- **Persistent Storage**: Conversation history is saved in SQLite database

## Requirements

- Python 3.8+
- phidata
- groq
- yfinance
- duckduckgo-search

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/financial-advisor-ai.git
   cd financial-advisor-ai
   ```

2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Set up your Groq API key:
   ```
   export GROQ_API_KEY=your_api_key_here
   ```

## Usage

Run the playground application:
```
python playground.py
```

This will start a local web server, typically at http://localhost:7777, where you can interact with both agents.

### Example Queries

For the Finance Agent:
- "What is the current price of AAPL?"
- "Show me analyst recommendations for TSLA"
- "Give me the latest news about Microsoft"
- "Compare the financial performance of AMZN and GOOG"

For the Web Agent:
- "What are the latest developments in cryptocurrency?"
- "Find information about recent changes in interest rates"
- "Search for upcoming IPOs in the tech sector"

## Project Structure

- `playground.py`: Main application file that configures and serves the AI agents
- `agents.db`: SQLite database that stores conversation history (created on first run)

## Customization

You can modify the agents' behavior by adjusting their configuration in `playground.py`:

- Change the model by updating the `model` parameter
- Add or remove tools from the `tools` list
- Modify instructions to change how agents respond
- Adjust storage settings for conversation history

## License

MIT

## Acknowledgments

- [phidata](https://github.com/phidatahq/phidata) for the AI agent framework
- [Groq](https://groq.com/) for the LLM API
- [YFinance](https://github.com/ranaroussi/yfinance) for financial data tools
- [DuckDuckGo Search](https://github.com/deedy5/duckduckgo_search) for web search capabilities


