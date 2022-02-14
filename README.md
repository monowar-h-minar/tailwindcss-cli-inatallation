# Tailwind CSS Installation Using- Tailwind CLI

The simplest and fastest way to get up and running with Tailwind CSS from scratch is with the Tailwind CLI tool

### 1. Install Tailwind CSS
Install tailwindcss via npm, and create your tailwind.config.js file.

```
1. npm install -D tailwindcss
2. npx tailwindcss init

```

### 2. Configure your template paths
Add the paths to all of your template files in your tailwind.config.js file.

```
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}

```


### 3. Start the Tailwind CLI build process
Run the CLI tool to scan your template files for classes and build your CSS.

```
npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch

```

### 4. Start using Tailwind in your HTML
Add your compiled CSS file to the <head> and start using Tailwind’s utility classes to style your content.

```
<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="/dist/output.css" rel="stylesheet">
</head>
<body>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
</body>
</html>
  
```



