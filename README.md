# PPT to JSON (Senior Project)

This project provides a simple and convenient way to convert PowerPoint (.ppt) files into JSON format. This allows for easy parsing, manipulation, and analysis of slide content.

## Resulting JSON structure

The resulting JSON object has a structure that represents the content of the PowerPoint file. Each slide in the file is converted into an object in the JSON array. Each object includes the content of the slide, formatted as a string, along with any additional metadata about the slide.

```json
[
  {
    "slideNumber": 1,
    "title": "Slide 1",
    "content": "This is the content of slide 1."
  },
  {
    "slideNumber": 2,
    "title": "Slide 2",
    "content": "This is the content of slide 2."
  },
  // More slides...
]
```

## Error Handling

If an error occurs while reading the PowerPoint file or converting it to JSON, the Promise will be rejected with an Error. You can handle this using the `.catch()` method:

```javascript
PPTtoJSON.readPath("./non_existent.ppt")
  .then((json) => console.log(json))
  .catch((error) => console.error(error.message)); // Will print: Error: File not found: ./non_existent.ppt
```

## Contributing

If you'd like to contribute, please fork the repository and use a feature branch. Pull requests are warmly welcome.

## Licensing

The code in this project is licensed under MIT license. See the [LICENSE](LICENSE) file for more information.
