# Setup

Learn how to set up your first Pebble project.

## Creating a New Project

To create a new Pebble project, run:

```bash
pebble init my-project
```

This will create a new directory with the basic project structure:

```
my-project/
├── pebble.config.js
├── src/
│   └── index.js
├── package.json
└── README.md
```

## Project Configuration

The `pebble.config.js` file is the main configuration file for your project:

```javascript
module.exports = {
  name: 'my-project',
  version: '1.0.0',
  // Add your configuration options here
};
```

## Navigate to Your Project

```bash
cd my-project
```

## Install Dependencies

Install the required dependencies:

```bash
npm install
```

## Verify Setup

Verify your project is set up correctly:

```bash
pebble verify
```

If everything is configured properly, you'll see a success message.

## Next Steps

Now that your project is set up, learn about [Basic Usage](basic-usage.md) to start working with Pebble.
