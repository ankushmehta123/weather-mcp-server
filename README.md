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


