
# Code Tool

Provides Code Blocks for the [Editor.js](https://editorjs.io).

![image](https://user-images.githubusercontent.com/6184465/64905642-0a125b80-d70e-11e9-875f-5240815e6290.png)


## Installation

### Install via NPM

Get the package

```shell
npm i --save-dev @groupher/editor-code
```

Include module at your application

```javascript
const Code = require('@groupher/editor-code');
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
    code: Code,
  },
  
  ...
});
```

## Output data

| Field     | Type     | Description          |
| --------- | -------- | -------------------- |
| text      | `string` | code's text         |
| lang   | `string` | code's language |


```json
{
    "type" : "quote",
    "data" : {
        "text" : ""body {  color: tomato;  margin-left: 20px;};",
        "lang" : "css"
    }
}
```
