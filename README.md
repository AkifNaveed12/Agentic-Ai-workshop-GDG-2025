# Agentic-AI-Workshop-GDG-2025

A hands-on workshop project demonstrating how to build AI agents using Google's Agent Development Kit (ADK) with Gemini models.

## Project Overview

This repository contains a practical implementation of an AI agent that leverages Google's ADK framework to create intelligent, tool-enabled agents. The workshop focuses on building agents that can reason about tasks, interact with external tools, and provide helpful responses to user queries.

## Features

- **Google Gemini Integration**: Uses the latest Gemini models (gemini-flash-latest)
- **Tool Calling**: Demonstrates how to create and use custom tools with agents
- **Real-world Examples**: Includes practical agent implementations

## Project Structure

```
.
├── README.md                 # This file
├── .gitignore               # Git ignore rules
└── my_agent/                # Main agent module
    ├── __init__.py          # Package initialization
    └── agent.py             # Agent implementation
```

## Getting Started

### Prerequisites

- Python 3.8+
- Google Cloud credentials for Gemini API access
- Virtual environment (recommended)

### Installation

1. Clone this repository:

```bash
git clone https://github.com/yourusername/Agentic-AI-Workshop-GDG.git
cd Agentic-AI-Workshop-GDG
```

2. Create and activate a virtual environment:

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

## Usage

The project includes a sample agent that tells the current time in specified cities:

```python
from my_agent.agent import root_agent

# Use the agent to answer queries
response = root_agent.process("What time is it in New York?")
```

## Agent Components

### `root_agent`

A specialized agent configured with:

- **Model**: Gemini Flash (optimized for speed and efficiency)
- **Capability**: Retrieves current time information for any city
- **Tool**: `get_current_time()` function for real-world data

## Development

### Running Tests

```bash
pytest tests/
```

### Building & Deployment

Follow the Google ADK documentation for deployment options and best practices.

## Key Learnings

- How to define and register custom tools for agents
- Agent instruction design and prompt engineering
- Integration with Gemini models
- Handling tool responses and result formatting

## Resources

- [Google Agent Development Kit Documentation](https://cloud.google.com/docs/agents)
- [Gemini API Reference](https://ai.google.dev/api)
- [Workshop Materials](link-to-materials)

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Google Cloud Agents team for the ADK framework
- GDG community for organizing the workshop
