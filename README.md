This repository contains a multi-component Python CLI utility for dynamically generating and executing unit tests, integrating with an in-memory key-value store, and analyzing dead code in Python applications. The architecture is designed to be modular, with a clear separation between core logic and the command-line interface. The tools are intended for use in production environments where robust testing and code analysis are critical.

## Architecture

### Core
- **Code Generation**: Dynamically generates unit tests based on code coverage.
- **Key-Value Store**: Manages an in-memory key-value store using SQLite.
- **API Stresstest**: Simultaneously sends asynchronous requests to APIs for stress testing.
- **Dead Code Analysis**: Identifies and analyzes dead code in the application.

### CLI
- **Interactive Interface**: Provides a rich terminal interface for user interaction.
- **Command Handling**: Handles various commands to interact with the core functionalities.

### Testing
- **Unit Tests**: Ensures the core functionalities work as expected.
- **Integration Tests**: Tests the interaction between the CLI and core functionalities.

## Usage

### Installation
```bash
pip install -r requirements.txt
```

### Running the CLI
```bash
dynamic-test-cli [command] [options]
```

### Example Commands
- **Generate Tests**: `dynamic-test-cli generate-tests -p path/to/project`
- **Stress Test API**: `dynamic-test-cli stress-api -u http://api.example.com`
- **Analyze Code**: `dynamic-test-cli analyze-code -p path/to/project`

## Contributing
Contributions are welcome! Please read the [CONTRIBUTING.md](CONTRIBUTING.md) file for details on how to contribute.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.