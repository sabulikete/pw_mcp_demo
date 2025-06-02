# Playwright MCP Demo

This repository contains test scripts for web application testing using Playwright and MCP (Model Context Protocol).

MCP (Model Context Protocol) is a framework that allows AI models like Claude to interact with browser automation tools such as Playwright, enabling AI-driven test execution without writing traditional code.

## Project Structure

- **TestRunner.md**: Main file for executing the test suites
- **TestSuites/**: Contains test case definitions for different features
- **TestData/**: Contains test data files
- **TestResults/**: Contains test execution reports

## Test Execution

The tests are designed to be executed according to priority and sequence defined in the TestRunner.md file. Test cases are organized by priority (High, Medium, Low) and will be run in the order specified in the TestRunner.md file.

The test execution follows this workflow:
1. Before each test case: Setup the test environment
2. Execute test steps: Follow test steps in each test case
3. After each test case: Clean up the environment
4. Generate a test report: Create an HTML report with results

## Prerequisites

- Playwright MCP (Refer the Playwright MCP documentation on how to set it up [Instructions](https://github.com/microsoft/playwright-mcp/blob/main/README.md))
- Browser: Chrome or any other browser supporting Playwright tests (as configured in the test settings)
- Visual Studio Code with GitHub Copilot Chat extension (v0.11.0 or later)
- Node.js (v16 or later) and npm

## How to Run
1. Clone this repository to your local machine
2. Make sure Playwright MCP is installed in VS Code (see Prerequisites)
3. Open the project in VS Code
4. Open the Copilot Chat panel and select Claude 3.7 Sonnet or Claude Sonnet 4 as the Copilot mode
5. Select the "TestRunner.md" file in the editor
6. In the Copilot agent chat, type "Run the test suite"
7. The AI will execute the tests according to the instructions in the test files
