# System Prompts

This directory contains system prompts used by Claude Code, Anthropic's official CLI for Claude.

## Files

### system_prompt_1.md
The main system prompt for Claude Code. It defines:
- Core functionality and behavior
- Security guidelines
- Response tone and style
- Proactiveness boundaries
- Code conventions and style guidelines
- Task management instructions
- Tool usage policies
- Environment information

### system_prompt_2.md
A specialized prompt for git history analysis. It instructs Claude to:
- Analyze file modification counts
- Return five frequently modified filenames representing core application logic
- Ensure diversity in the returned filenames

### system_prompt_3.md
A prompt for conversation topic detection. It instructs Claude to:
- Analyze if a message indicates a new conversation topic
- Extract a 2-3 word title for new topics
- Return results in JSON format

### system_prompt_4.md
A prompt for conversation summarization. It instructs Claude to:
- Summarize coding conversations in under 50 characters
- Capture main tasks, key files, problems addressed, and current status

## Usage

These system prompts define Claude Code's behavior and capabilities when interacting with users through the CLI interface. They provide the foundation for Claude's understanding of how to assist with software engineering tasks effectively.
