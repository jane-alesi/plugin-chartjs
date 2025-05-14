# satware® AI Chart JS Plugin

A Chart.js plugin for satware.ai and TypingMind, enabling dynamic chart rendering directly within the chat interface using a JavaScript implementation.

## Features

*   Generates various Chart.js chart types (Bar, Line, Pie, Doughnut, etc.)
*   Customizable data, labels, and Chart.js options.
*   Implemented directly in JavaScript for client-side rendering via the chat platform's HTML rendering capabilities.

## Installation

1.  Go to the Plugins section in your TypingMind or chat.satware.ai instance.
2.  Click "Import plugins".
3.  Select "Import from GitHub".
4.  Enter the repository URL: `https://github.com/jane-alesi/plugin-chartjs`
5.  Click Import.

## Usage

The plugin exposes a function `render_chart` with the following parameters:

*   `title` (string): The title of the chart.
*   `chartType` (string): The type of chart (e.g., "bar", "line", "pie"). See the `plugin.json` `openaiSpec` for a full list of supported types.
*   `data` (object): The chart data, including `labels` (array of strings) and `datasets` (array of objects, each with `label` and `data` array of numbers).
*   `options` (object): An object containing standard Chart.js configuration options, such as `scales`, `plugins` (legend, tooltip), `responsive`, etc. Refer to the `plugin.json` `openaiSpec` for currently supported options.

Your AI model should be able to generate calls to this function based on user requests for data visualization.

## Development

This plugin is developed adhering to FOSS principles. Contributions are welcome via pull requests.

### File Structure

*   `plugin.json`: The plugin manifest and OpenAPI specification.
*   `implementation.js`: The JavaScript code implementing the `render_chart` function.
*   `README.md`: This documentation.

## License

[Specify a FOSS license, e.g., MIT, Apache 2.0, GPL]

## Contributing

[Optional: Add details on how to contribute]
