# Software Testing Agent

## Overview

Software Testing Agent is an AI-powered agent designed to automate software testing processes.

It analyzes source code, understands project structure and dependencies, generates test cases, executes tests, investigates failures, and provides detailed testing reports.

The agent supports two main usage modes:

- **GitHub Integration:** Analyze repositories and test code at the project level.
- **IDE Integration:** Test individual files, functions, or selected code directly from the development environment.

The initial implementation will focus on Python projects, with the possibility of supporting additional programming languages in future versions.

## Core Features

- **Code Analysis:** Understand source code, functions, classes, and project structure.
- **Test Planning:** Identify important test scenarios and edge cases.
- **Test Generation:** Generate test cases based on the analyzed code.
- **Automated Execution:** Run generated tests using Pytest.
- **Failure Analysis:** Investigate failed tests and identify potential causes.
- **Coverage Analysis:** Evaluate test coverage and identify untested code.
- **Testing Reports:** Provide structured reports containing test results, failures, and recommendations.

## Agent Workflow

1. Receive a testing request.
2. Analyze the target code and its dependencies.
3. Identify test scenarios and edge cases.
4. Generate appropriate test cases.
5. Execute tests using the available testing tools.
6. Analyze failures and investigate their causes.
7. Evaluate code coverage.
8. Generate a final testing report.

## Tools

The agent will use a collection of tools to interact with source code and execute testing operations.

| Tool | Description |
|---|---|
| `list_files` | List files and directories in the project. |
| `read_file` | Read source code and configuration files. |
| `search_code` | Search for functions, classes, and code references. |
| `get_dependencies` | Identify project dependencies and installed packages. |
| `generate_tests` | Generate test cases for the target code. |
| `run_tests` | Execute tests using Pytest. |
| `analyze_failures` | Analyze failed tests and investigate potential causes. |
| `get_coverage` | Retrieve code coverage information. |

## Technology Stack

| Component | Technology |
|---|---|
| Programming Language | Python |
| Agent Framework | LangGraph |
| LLM | Qwen3-Coder Family |
| LLM Provider | OpenRouter |
| Testing Framework | Pytest |
| Coverage Analysis | Coverage.py |

**LLM Note:** The project will initially use a suitable free model available through OpenRouter. The exact model will be selected based on coding capabilities, tool-calling support, and availability.

## Project Goals

The main goal is to build an intelligent testing agent that reduces manual testing effort and improves software testing workflows.

Future improvements may include:

- Advanced GitHub repository integration.
- IDE extensions for direct code testing.
- Multi-language support.
- Regression testing.
- Automated bug reproduction.
- Suggested code fixes.
- More advanced testing strategies.

## Project Status

**Status:** Initial Planning & Development

The first version will focus on Python code analysis, test generation, automated execution, and failure analysis. Additional integrations and capabilities will be introduced incrementally.
