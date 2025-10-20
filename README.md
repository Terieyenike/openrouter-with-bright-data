# Jupyter Notebook: LangChain with Bright Data MCP Server

A Jupyter notebook demonstrating the integration of LangChain with Bright Data's MCP (Model Context Protocol) server for advanced web scraping and search capabilities.

## Overview

This project showcases how to use LangChain's ReAct agent framework with Bright Data's web scraping tools through their MCP server. The notebook demonstrates creating an intelligent web search agent that can:

- Search across multiple search engines (Google, Bing, Yandex)
- Scrape web content with advanced bot detection bypass
- Handle complex web interactions through browser automation
- Process structured data from major platforms

## Features

### Available Tools
- **search_engine**: Get search results from Google, Bing, or Yandex
- **scrape_as_markdown**: Extract content from any webpage with bot detection bypass
- **search_engine_batch**: Run multiple search queries simultaneously
- **scrape_batch**: Scrape multiple webpages in parallel

### Key Capabilities
- **Advanced Web Scraping**: Bypass bot detection and CAPTCHAs
- **Multi-Platform Support**: Structured extractors for major platforms (Amazon, LinkedIn, Instagram, Facebook, X, TikTok, YouTube, Reddit, Zillow, etc.)
- **Browser Automation**: Navigate, click, type, and take screenshots for complex interactions
- **Batch Processing**: Handle multiple operations efficiently
- **ReAct Agent**: Intelligent decision-making for tool selection and execution

## Prerequisites

- Python 3.8+
- Jupyter Notebook or JupyterLab
- Bright Data API token
- OpenRouter API key (or OpenAI API key)

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Terieyenike/openrouter-with-bright-data
   cd openrouter-with-bright-data
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up environment variables:**
   Create a `.env` file in the project root:
   ```env
   BRIGHT_DATA_API_TOKEN=your_bright_data_token_here
   OPENROUTER_API_KEY=your_openrouter_api_key_here
   ```

## Usage

1. **Start Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

2. **Open the notebook:**
   - Open `main.ipynb`
   - Run all cells to see the agent in action

3. **Test the agent:**
   The notebook includes a test query: "Search for the latest news about AI agents with its relevant tools"

## Project Structure

```
jn-langchain-with-brightdatamcp/
├── main.ipynb          # Main Jupyter notebook
├── requirements.txt    # Python dependencies
├── README.md          # This file
└── .env               # Environment variables (create this)
```

## Dependencies

- **langchain-mcp-adapters**: MCP client adapters for LangChain
- **langchain-openai**: OpenAI integration for LangChain
- **langgraph**: Graph-based agent framework
- **python-dotenv**: Environment variable management
- **anthropic**: Anthropic AI models support

## Configuration

### Bright Data Setup
1. Sign up for a Bright Data account
2. Get your API token from the dashboard
3. Add it to your `.env` file

### OpenRouter Setup
1. Sign up for OpenRouter
2. Get your API key
3. Add it to your `.env` file

## Example Usage

The notebook demonstrates creating a ReAct agent that can:

```python
# Example query
"Search for the latest news about AI agents with its relevant tools"
```

The agent will:
1. Analyze the query
2. Choose appropriate tools (search_engine, scrape_as_markdown)
3. Execute the tools
4. Process and present the results

## Advanced Features

### Structured Data Extraction
The agent can extract structured data from:
- E-commerce sites (Amazon, eBay)
- Social media (Instagram, Facebook, X, TikTok)
- Professional networks (LinkedIn)
- Real estate (Zillow)
- Discussion forums (Reddit)
- Video platforms (YouTube)

### Error Handling
- Graceful handling of rate limits
- Automatic retry mechanisms
- Comprehensive error logging

## Troubleshooting

### Common Issues

1. **Missing API Keys**: Ensure both `BRIGHT_DATA_API_TOKEN` and `OPENROUTER_API_KEY` are set in your `.env` file

2. **Import Errors**: Make sure all dependencies are installed:
   ```bash
   pip install -r requirements.txt
   ```

3. **Connection Issues**: Check your internet connection and API token validity

### Logging
The notebook includes logging configuration to filter out verbose SSE connection messages for cleaner output.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is open source. Please check the repository for license details.

## Support

For issues and questions:
- Check the [Bright Data documentation](https://docs.brightdata.com/introduction)
- Review [LangChain documentation](https://python.langchain.com/)
- Open an issue in this repository

## Acknowledgments

- [Bright Data](https://brightdata.com/) for web scraping infrastructure
- [LangChain](https://langchain.com/) for the agent framework
- [OpenRouter](https://openrouter.ai/) for LLM access
