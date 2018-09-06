# \<markdown-editor\>

[CodeMirror](http://www.codemirror.net)'s markdown mode into web components

## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) and npm (packaged with [Node.js](https://nodejs.org)) installed. Run `npm install` to install your element's dependencies, then run `polymer serve` to serve your element locally.

## Viewing Your Element

```
$ polymer serve
```

## Usage

Basic usage
```html
<markdown-editor></markdown-editor>
```

Set text content
```html
<markdown-editor content="# New Document"></markdown-editor>
```

Event listener when text is updated
```html
<markdown-editor></markdown-editor>
<script>
  document.querySelector('markdown-editor').addEventListener('change', function (e) {
      console.log(e.detail.getValue());
  })
</script>
```
`e.detail.getValue()` is text content

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.
