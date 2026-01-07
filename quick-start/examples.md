# Examples

Explore practical examples to help you understand how to use Pebble effectively.

## Example 1: Hello World

The simplest Pebble project:

```javascript
// src/index.js
export default function hello() {
  return 'Hello, Pebble!';
}
```

Run it:

```bash
pebble dev
```

## Example 2: Configuration with Environment Variables

Use environment-specific configurations:

```javascript
// pebble.config.js
module.exports = {
  name: 'my-app',
  environment: process.env.NODE_ENV || 'development',
  api: {
    url: process.env.API_URL || 'http://localhost:4000'
  }
};
```

## Example 3: Custom Build Configuration

Customize your build process:

```javascript
// pebble.config.js
module.exports = {
  build: {
    outDir: 'build',
    minify: true,
    sourcemap: true,
    target: 'es2020'
  }
};
```

## Example 4: Multi-Page Application

Structure for a multi-page app:

```
my-app/
├── src/
│   ├── pages/
│   │   ├── home.js
│   │   ├── about.js
│   │   └── contact.js
│   └── index.js
└── pebble.config.js
```

## Example 5: Integration with External APIs

```javascript
// src/api.js
export async function fetchData() {
  const response = await fetch('https://api.example.com/data');
  return response.json();
}
```

## More Examples

For more comprehensive examples and templates, visit:

* [Official Examples Repository](https://github.com/pebble/examples)
* [Community Showcases](https://pebble.dev/showcase)

## Next Steps

Now that you've seen some examples, explore the [Additional Resources](../resources/README.md) for more in-depth documentation.
