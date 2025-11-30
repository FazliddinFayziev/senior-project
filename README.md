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
