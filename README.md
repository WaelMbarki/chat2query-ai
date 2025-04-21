A natural language interface for querying a retail management database using local LLM technology.

## Overview
This backoffice chatbot allows users to query a retail database using natural language. It translates user questions into SQL queries, executes them against the database, and returns human-readable responses. The system respects user roles and permissions, ensuring users only access data they're authorized to see.

## Features
- Natural language to SQL translation
- Role-based access control
- Local LLM processing using Ollama
- Error recovery with automatic query correction
- Human-friendly response formatting
## Requirements
- Python 3.8+
- MySQL database
- Ollama with the Mistral model installed

## How It Works
1. The system captures the user's natural language query
2. It retrieves the user's role and permissions
3. The LLM generates an appropriate SQL query based on the request and user's access level
4. The query is executed against the database
5. Results are transformed into a natural language response
6. If a query fails, the system attempts to correct it automatically
