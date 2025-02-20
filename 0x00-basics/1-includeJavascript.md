# Javascript
There are two types of JavaScript:

- Internal
- External

## Internal Javascript

   It refers to a JavaScript code that is written directly within an HTML file, usually inside a `script` tag.
   ```
   <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript</title>
</head>
<body>
    <script>
        console.log("Hi there");
    </script>
</body>
</html>
```
## External Javascript
It refers to a JavaScript file that is placed in a separate .js file.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript</title>
</head>
<body>
    <script src="test.js"></script>
</body>
</html>
```
In the JavaScript console, the code will be as follows:
```
console.log("Javascript is fun") 
```
### Optimizing script loading
Javascript can stop a page from rendering if it is not loaded correctly. This is because websites parses the HTML code line by line and when it comes across a resource that needs to be downloaded to the page e.g. an image or video, it sends the request to the server to download the resource. However, when it comes across the `script` tag to download Javascript, it stops until the Javascript is downloaded, it then executes the downloaded Javascript and then continues to parse the HTML. 

This can hurt the website loading speed. To counter this and improve on performance, we use;

1. `defer` keyword. This ensures that the scripts are loaded once the HTML is fully parsed.
```
<script src="test.js" defer></script>
```

   


