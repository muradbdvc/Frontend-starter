# frontend starter theme
just clone & use

```bash
# Clone the Git repository
git clone ...

# # Install PHP-composer dependencies [It's empty]

# Install node module packages
npm i

# Start development mode
npm start
```

sass code generate

create style.scss & hit the command

```bash

sass source/style.scss source/style.css
```
add the extension in vs code

Live Sass Compiler
v6.1.2
Glenn Marks
1,674,932
(57)
Compile Sass or Scss to CSS at realtime.

# Add the paths to all of your template files in your tailwind.config.js file.

```bash
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```
# Add the Tailwind directives to your CSS
Add the @tailwind directives for each of Tailwind’s layers to your main CSS file.
into assets/style.css 
```bash
@tailwind base;
@tailwind components;
@tailwind utilities;

```

# Start the Tailwind CLI build process
Run the CLI tool to scan your template files for classes and build your CSS.

```bash
npx tailwindcss -i ./assets/style.css -o ./assets/style.css --watch
```

# Start using Tailwind in your HTML
Add your compiled CSS file to the <head> and start using Tailwind’s utility classes to style your content.

```bash
<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="./style.css" rel="stylesheet">
</head>
<body>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
</body>
</html>
```