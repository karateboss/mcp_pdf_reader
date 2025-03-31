# mcp-pdf-reader
Model Context Protocol (MCP) server to read a single pdf document

## Installation

### Prerequisites

#### Windows
1. Install Claude Desktop (or another MCP-enabled AI tool)
   - Download [Claude for Desktop](https://claude.ai/download) 
   - Follow the current installation instructions: [Installing Claude Desktop](https://support.anthropic.com/en/articles/10065433-installing-claude-for-desktop)
     
2. Install Python 3.10 or higher:
   - Download the latest Python installer from [python.org](https://python.org)
   - Run the installer, checking "Add Python to PATH"
   - Open Command Prompt and verify installation with `python --version`

3. Install uv:
   - Open Command Prompt as Administrator
   - Run `pip install --user uv`
   - Verify installation with `uv --version`

#### macOS
1. Install Claude Desktop (or another MCP-enabled AI tool)
   - Download [Claude for Desktop](https://claude.ai/download) 
   - Follow the current installation instructions: [Installing Claude Desktop](https://support.anthropic.com/en/articles/10065433-installing-claude-for-desktop)
     
2. Install Python 3.10 or higher:
   - Using Homebrew: `brew install python`
   - Verify installation with `python3 --version`

3. Install uv:
   - Using Homebrew: `brew install uv`
   - Alternatively: `pip3 install --user uv`
   - Verify installation with `uv --version`

## Configuration

Add the following to your `claude_desktop_config.json`:

```json
{
    "mcpServers": {
        "mcp-pdf-reader": {
            "command": "uvx",
            "args": [
                "--from",
                "git+https://github.com/karateboss/mcp-pdf-reader@main",
                "read_pdf"
            ]
        }
    }
}
```
## Attribution

This software package implements the ability to read a pdf file into a MCP enabled framework and is developed by [Safe Swiss Cloud](https://safeswisscloud.com). 

## License

This software is licensed under the Attribution-ShareAlike 4.0 International license from Creative Commons Corporation ("Creative Commons"). 

This means you are free to:
- Share: Copy and redistribute the material in any medium or format
- Adapt: Remix, transform, and build upon the material for any purpose, even commercially

Under the following terms:
- Attribution: You must give appropriate credit to Safe Swiss Cloud, provide a link to the license, and indicate if changes were made
- ShareAlike: If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original

For the full license text, visit: [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/)

## Contributing

We welcome contributions to improve these tools. Please submit issues and pull requests through our repository.

## Support

For questions and support:
1. Check our documentation
2. Submit an issue in our repository
