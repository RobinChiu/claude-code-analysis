# Tools CSV Documentation

This repository contains a `tools.csv` file that defines a collection of tools available for use with AI assistants or automation systems. The file serves as a configuration source for available tools, their descriptions, and parameter specifications.

## File Structure

The `tools.csv` file has the following columns:

1. **Index** - A numeric identifier for each tool
2. **Name** - The name of the tool
3. **Description** - A detailed description of the tool's purpose, functionality, and usage guidelines
4. **Parameters** - JSON schema definition of the tool's parameters

## Available Tools

The file currently defines 14 tools:

1. **Task** - Launches a new agent to handle complex, multi-step tasks autonomously
2. **Bash** - Executes bash commands in a persistent shell session
3. **Glob** - Fast file pattern matching tool for finding files by name patterns
4. **Grep** - Powerful search tool built on ripgrep for searching file contents
5. **LS** - Lists files and directories in a given path
6. **ExitPlanMode** - Used to exit plan mode when ready to implement a solution
7. **Read** - Reads files from the local filesystem
8. **Edit** - Performs exact string replacements in files
9. **MultiEdit** - Makes multiple edits to a single file in one operation
10. **Write** - Writes content to files in the local filesystem
11. **NotebookEdit** - Edits cells in Jupyter notebooks
12. **WebFetch** - Fetches and processes content from specified URLs
13. **TodoWrite** - Creates and manages structured task lists for coding sessions
14. **WebSearch** - Allows searching the web for up-to-date information

## Usage

This tools.csv file can be imported into systems that support tool-based interactions with AI assistants. Each tool has specific parameters and usage guidelines detailed in its description.

### Example Tool Usage

For example, to use the **Grep** tool:

```json
{
  "pattern": "function searchData",
  "path": "/path/to/search",
  "glob": "*.js",
  "output_mode": "content"
}
```

## Parameter Schemas

Each tool has a specific parameter schema defined in JSON Schema format. These schemas specify:

- Required and optional parameters
- Parameter types and formats
- Parameter descriptions
- Default values (where applicable)

## Best Practices

When using these tools:

1. Read the full description of each tool to understand its capabilities and limitations
2. Follow the usage guidelines provided in the tool descriptions
3. Provide all required parameters as specified in the parameter schemas
4. Use the appropriate tool for each specific task

## Contributing

To add new tools or modify existing ones, update the tools.csv file following the established format:
- Maintain the column structure
- Provide detailed descriptions
- Define complete parameter schemas using JSON Schema format
