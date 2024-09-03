# jsonexporter

`jsonexporter` is a simple Node.js package that helps you log user data to a JSON file. It provides a function `parseJSON` that allows you to parse key-value pairs from a string and store them in a specified JSON file.

## Features

- **Parse Input Strings**: Converts input strings containing key-value pairs into JSON format.
- **Custom File Paths**: Optionally specify a custom file path to save the JSON data.
- **Automatic Data Conversion**: Converts strings like `"true"`, `"false"`, and numeric strings into their corresponding boolean and number types.

## Setup

First, make sure you have Node.js installed. Then, you can include `jsonexporter` in your project by copying the `parseJSON` function into your codebase.

### Install Dependencies

```bash
npm init -y
npm install fs
```
**They are preinstalled with the `package for node.js` but install it if it doesn't work as intended.**

### JSON file setup

First, `Create a .json file` mine here is called demo.json.

Then add a `{}` to your `.json` file

```json
{}
```

### Usage

```javascript
parseJSON("user: Cooler, val1: Value, Val2: Value...", "./demo.json") //An infinite amount of values can be added and make sure to use the "user" attribute and replace <filepath> with your actual file path example: ./data.json!
```

output:

```console
-----------------------------
User data added/updated successfully.
Logs {
  Update: "Modified ./data.json
  key="undefined"
}
-----------------------------
```

demo.json:

```json
{
    "Cooler": {
        "val1": "Value",
        "Val2": "Value..."
    }
}
```

## Contributing
If you'd like to contribute to `jsonexporter`, please fork the repository and use a feature branch. Pull requests are welcome.

## LICENSE
This project is licensed under the [MIT License](github.com/CoolerHub/parseJSON#License).
