# Basic Usage

Learn the fundamental commands and workflows for working with Pebble.

## Core Commands

### Start Development Server

Run the development server:

```bash
pebble dev
```

This starts a local development server with hot-reloading enabled.

### Build Your Project

Create a production build:

```bash
pebble build
```

The build output will be placed in the `dist/` directory.

### Run Tests

Execute your test suite:

```bash
pebble test
```

### Deploy

Deploy your project:

```bash
pebble deploy
```

## Common Workflows

### Development Workflow

1. Start the development server: `pebble dev`
2. Make changes to your code
3. View changes automatically in your browser
4. Run tests: `pebble test`

### Production Workflow

1. Build your project: `pebble build`
2. Test the production build
3. Deploy: `pebble deploy`

## Configuration Options

You can customize Pebble's behavior through the `pebble.config.js` file:

```javascript
module.exports = {
  port: 3000,
  build: {
    outDir: 'dist',
    minify: true
  },
  dev: {
    hot: true,
    open: true
  }
};
```

## Getting Help

For more information on any command, use the `--help` flag:

```bash
pebble --help
pebble build --help
```

## Next Steps

Check out [Examples](examples.md) for practical use cases and sample projects.
