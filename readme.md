# Cron Expression Parser

This project is a command-line application designed to parse cron strings and expand each field to show the times at which the cron job will run. The application is written in JavaScript and does not rely on existing cron parser libraries, showcasing the ability to create a custom solution.

## Features

- Parses standard cron format with five time fields (minute, hour, day of month, month, and day of week) plus a command.
- Outputs the parsed cron string as a table with field names and times.
- Handles a subset of cron strings correctly, prioritizing functionality over handling all possible cron strings.



## Running the Application

### Using Node

#### Installing Node.js and npm

1. **Download Node.js**: Visit [https://nodejs.org/](https://nodejs.org/) and download the installer for your operating system. The Node.js installer includes npm, so you don't need to install it separately.
2. **Run the Installer**: Open the downloaded file and follow the prompts to install Node.js and npm. The default settings are recommended for most users.
3. **Verify Installation**: Open a terminal or command prompt and run the following commands to verify that Node.js and npm are installed correctly: `node -v` `npm -v`. These commands should display the versions of Node.js and npm installed on your system.

#### Installing Jest Globally

Jest is a testing framework for JavaScript. To install Jest globally, run the following command in your terminal or command prompt: `npm install -g jest`. This command installs Jest globally, making it available for all projects on the system.

#### Debugging

1. **Open the Project Directory**: Navigate to the project directory in your terminal.
2. **Run the Application**: Execute the application by running `node cron_parser_command.js "your_cron_string_here command"`. Replace `"your_cron_string_here"` with the cron string you wish to parse and `command` with your suitable command.
3. This project includes a set of tests to ensure the parser functions correctly. To run the tests, execute `jest` in the project directory.

### Using the HTML Interface

If you want to skip installation and only want to play around with cron strings, you can open `index.html` in your browser. This provides a simple interface for testing cron strings without needing to install anything. Here's how to do it:

1. **Open the HTML File**: Locate the `index.html` file in the project directory. You can do this by navigating to the project folder in your file explorer or terminal.
2. **Open in a Browser**: Double-click the `index.html` file to open it in your default web browser. Alternatively, you can right-click the file and select "Open with" followed by your preferred web browser.
3. **Use the Interface**: Once the HTML page is open in your browser, you'll see a form where you can enter your cron expression. You can also specify the number of occurrences you want to see and a reference date for the calculation. After filling in the details, click the "Parse" button to see the parsed cron string in a table format.
4. **Experiment with Different Cron Strings**: Feel free to experiment with different cron strings to see how they are parsed and expanded. This can be a great way to understand how cron expressions work and how they can be broken down into their component parts.

#### Note

- The HTML interface is designed for quick testing and does not require any server-side processing. All parsing is done in the browser using JavaScript.
- If you're interested in the code behind the HTML interface, you can explore the `cron_parser.js` file in the project directory.


## Project Directory Overview

Below is a detailed overview of the project's directory structure, highlighting the purpose of each component within the project. The structure is designed to facilitate easy navigation and understanding for developers working on or with this project.

### Directory Layout

```
cron-parser/
├── coverage/                  # Contains test coverage reports
├── cron_parser.js             # Core JavaScript file for parsing cron strings
├── cron_parser.test.js        # Test suite for the cron parser
├── cron_parser_command.js     # Command-line interface for the cron parser
├── index.html                 # HTML interface for testing cron strings
├── index.js                   # Entry point for the HTML interface
├── jest.config.js             # Jest testing framework configuration file
├── readme.md                  # Overview of the project, setup, and usage examples
└── styles.css                 # CSS styles for the HTML interface
```

### File Descriptions

- **`coverage/`**: Stores test coverage reports, helping ensure code quality and reliability. This is auto generated when `jest` command is run.
- **`cron_parser.js`**: Implements the logic to parse cron strings and output their schedules.
- **`cron_parser.test.js`**: Contains tests for verifying the functionality of `cron_parser.js`.
- **`cron_parser_command.js`**: Provides a CLI to interact with the cron parser, facilitating direct command-line usage.
- **`index.html`**: A simple HTML interface that allows users to test cron string parsing without needing any installation.
- **`index.js`**: Serves as the starting point for the HTML interface, initializing the application.
- **`jest.config.js`**: Configuration file for the Jest testing framework, specifies testing parameters.
- **`readme.md`**: Offers a comprehensive overview of the project, including setup instructions and usage examples.
- **`styles.css`**: Defines CSS styles for the HTML interface, ensuring a user-friendly visual presentation.


