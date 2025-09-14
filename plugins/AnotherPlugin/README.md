# AnotherPlugin

An advanced plugin demonstrating integration capabilities and complex features for LAO.

## Description

AnotherPlugin showcases more advanced plugin development patterns, including API integrations, configuration management, and pre-built binary distribution. This plugin serves as an example for developers building more complex LAO extensions.

## Features

- RESTful API integration
- Advanced configuration management
- Environment variable support
- Pre-built binary distribution
- Comprehensive logging
- Error handling and recovery

## Installation

### Option 1: From Source
1. Clone the plugin repository
2. Install dependencies: `npm install`
3. Build the plugin: `npm run build`
4. Configure LAO to load this plugin

### Option 2: Pre-built Binary
1. Download the latest release from the [releases page](https://github.com/example/another-plugin/releases/latest)
2. Extract to your LAO plugins directory
3. Configure as needed

## Configuration

Create a `config.json` file with the following structure:

```json
{
  "api_endpoint": "https://api.example.com",
  "timeout": 5000,
  "retry_attempts": 3,
  "features": {
    "caching": true,
    "compression": true
  }
}
```

### Environment Variables

Set the following environment variables:

- `API_KEY`: Your API authentication key
- `BASE_URL`: Base URL for the service (optional)

## Usage

```javascript
const AnotherPlugin = require('another-plugin');

const plugin = new AnotherPlugin({
  configPath: './config.json'
});

plugin.initialize()
  .then(() => plugin.execute())
  .catch(err => console.error('Plugin error:', err));
```

## API Reference

### Methods

- `initialize()`: Initialize the plugin with configuration
- `execute()`: Run the main plugin functionality
- `cleanup()`: Clean up resources and connections

### Events

- `ready`: Fired when plugin is ready
- `error`: Fired on errors
- `data`: Fired when data is received

## Development

To contribute to this plugin:

1. Fork the repository
2. Install development dependencies: `npm install --dev`
3. Run tests: `npm test`
4. Create a feature branch
5. Make your changes
6. Ensure tests pass
7. Submit a pull request

## License

This plugin is licensed under the Apache License 2.0. See the LICENSE file for details.

## Support

For support:
- Check the [documentation](https://another-plugin.readthedocs.io)
- Open an issue on GitHub
- Join the LAO community discussions