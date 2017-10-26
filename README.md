[![npm version](https://badge.fury.io/js/swagger-ui-cornify.svg)](https://badge.fury.io/js/swagger-ui-cornify)

# swagger-ui-cornify

Cornify plugin for Swagger-UI v3.

This is a lighthearted example of how to create an external plugin for Swagger-UI. This project has a minimal Webpack build pipeline that creates bundles for browser consumption.

The plugin is available on npm as `swagger-ui-cornify`, and minified release copies are attached to each [GitHub Release](https://github.com/shockey/swagger-ui-cornify/releases).

If you use the script directly, the module will be exposed on the global scope as `SwaggerUICornify`.

### How to use

Load this plugin (either through npm or directly), and provide it to Swagger-UI when you call it:

```js
SwaggerUI({
  url: "http://petstore.swagger.io/v2/petstore.yaml",
  plugins: [
    SwaggerUICornify
  ]
})
```

If/when the API definition you're viewing contains an `x-cornify: true` statement, magic will happen.
