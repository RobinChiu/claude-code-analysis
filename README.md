# Claude Code Analysis

This repository contains configuration and system files for Claude Code, Anthropic's official CLI for Claude. It provides the foundation for Claude's understanding and capabilities when interacting with users through the CLI interface.

## Repository Structure

### [system_prompt/](system_prompt/)

Contains system prompts that define Claude Code's behavior and capabilities:

- **system_prompt_1.md**: Main system prompt defining core functionality, security guidelines, response style, and more
- **system_prompt_2.md**: Specialized prompt for git history analysis
- **system_prompt_3.md**: Prompt for conversation topic detection
- **system_prompt_4.md**: Prompt for concise conversation summarization

[More details](system_prompt/README.md)

### [user_messages/](user_messages/)

Contains system reminder templates that are automatically inserted into user messages:

- **before.md**: Reminders inserted at the beginning of user messages
- **after.md**: Reminders inserted at the end of user messages

[More details](user_messages/README.md)

### [tools/](tools/)
![image](https://github.com/RobinChiu/claude-code-analysis/blob/main/image/tools.png)

Contains tool definitions for AI assistants:

- **tools.csv**: Defines 14 tools available for use with AI assistants, including their descriptions and parameter specifications

[More details](tools/README.md)

## Purpose

This repository serves as the configuration backbone for Claude Code, defining:

1. **System Behavior**: How Claude should respond, what tone to use, and what actions to take
2. **User Interaction**: How to process and augment user messages with system reminders
3. **Available Tools**: What tools Claude can use to assist with software engineering tasks

Together, these components enable Claude Code to function as an effective CLI tool for software engineering tasks, providing consistent behavior aligned with Anthropic's guidelines and user expectations.
