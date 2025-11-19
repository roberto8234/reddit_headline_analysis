# Visuals Folder

This folder contains HTML files for each visualization tab.

## Files Structure

- `visual1.html` - Visualization 1
- `visual2.html` - Visualization 2
- `visual3.html` - Visualization 3
- `visual4.html` - Visualization 4
- `visual5.html` - Visualization 5 (uses data1.json and data2.json)

## Adding Your Visualizations

1. Place your HTML files in this folder with the names listed above
2. Each HTML file should be a complete, standalone HTML document
3. For visual5.html, you can reference the JSON files using relative paths:
   - `../data1.json`
   - `../data2.json`

## Example HTML File Structure

```html
<!DOCTYPE html>
<html>
<head>
    <title>Visualization</title>
    <style>
        /* Your styles here */
    </style>
</head>
<body>
    <!-- Your visualization content here -->
    <script>
        // Your JavaScript here
    </script>
</body>
</html>
```

## Example for visual5.html (using JSON data)

```javascript
// Fetch the JSON data
fetch('../data1.json')
    .then(response => response.json())
    .then(data => {
        console.log('Data from data1.json:', data);
        // Use the data for your visualization
    });

fetch('../data2.json')
    .then(response => response.json())
    .then(data => {
        console.log('Data from data2.json:', data);
        // Use the data for your visualization
    });
```
