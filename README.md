# Weather MCP Server

## Overview

This project implements a Model Context Protocol (MCP) server that allows AI assistants (such as Claude) to interact with the National Weather Service (NWS) API. The server provides real-time weather alerts and forecasts for a given location.

## Features

- Retrieve active weather alerts for a given US state.
- Fetch weather forecasts for a specified latitude and longitude.
- Implements the FastMCP framework to expose tools for AI interaction.

## Technologies Used

- Python
- FastMCP
- httpx (for asynchronous HTTP requests)

## Prerequisites

Before running this project, ensure you have:

- Python installed (version 3.11.6 or higher recommended)
- uv package manager (pip install uv)
- httpx installed (pip install httpx)
- fastmcp installed (pip install fastmcp)
- Claude Desktop app

uv Package Manager Installation 
```bash
# On macOS and Linux.
curl -LsSf https://astral.sh/uv/install.sh | sh
```

```bash
# On Windows.
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```
Add to PATH

## Installation & Setup

1. Clone the repository:
   `git clone https://github.com/ankushmehta123/weather-mcp-server.git`

3. Install dependencies:
   `pip install -r requirements.txt`

5. Configure your MCP server by adding the following to
   ```claude_desktop_config.json:```
   ```{
    "mcpServers": {
        "weather": {
            "command": "C:/Users/"enter_your_username"/.local/bin/uv.exe",
            "args": [
                "--directory",
                "directory_location of main.py",
                "run",
                "main.py"
            ]
        }
    }
   }

## Usage

Run main.py
```python main.py```

### Available API Tools

Open Claude Desktop, you would see: 2 MCP tools available (at right-side of the search-bar)

<img height=200px, width=200px>![Screenshot 2025-03-15 132217](https://github.com/user-attachments/assets/d3d2a756-a416-4236-99f8-21884139fc03)</img>

<img>![Screenshot 2025-03-15 132224](https://github.com/user-attachments/assets/459d881b-47c8-4b9a-9ede-a270c21d54e7)</img>


You can ask real-time weather related questions to claude now:

<img>![Screenshot 2025-03-15 132527](https://github.com/user-attachments/assets/dba04376-f3ca-479a-81d8-8671df29d60d)</img>


