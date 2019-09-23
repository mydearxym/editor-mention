
# Mention Tool

Provides Code Blocks for the [Editor.js](https://editorjs.io).

![image](https://user-images.githubusercontent.com/6184465/65400436-c0ec9680-ddf4-11e9-9b18-6820a436d9c1.png)


## Installation

### Install via NPM

Get the package

```shell
npm i --save-dev @groupher/editor-mention
```

Include module at your application

```javascript
const Mention = require('@groupher/editor-mention');
```

### Download to your project's source dir

1. Upload folder `dist` from repository
2. Add `dist/bundle.js` file to your page.

## Usage

Add a new Tool to the `tools` property of the Editor.js initial config.

```javascript
var editor = EditorJS({
  ...
  
  tools: {
    ...
    mention: Mention,
  },
  
  ...
});
```

## Output data

| Field     | Type     | Description          |
| --------- | -------- | -------------------- |
| text      | `string` | code's text         |


```json
{
    "type" : "text",
    "data" : {
        "text" : "hello <span class=\"cdx-mention\">mydearxym</span>"
    }
}
```
