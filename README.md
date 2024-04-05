# Netlify-Node

PHP on AWS Lambda or Netlify

## Usage

```javascript
const path = require('path');
const netlify_node = require('netlify-node');

exports.handler = async function (event, context, callback) {
  const pathToWP = path.join(process.cwd(), 'wp');

  return await netlify_node({ docRoot: pathToWP, event: event });
}
```
