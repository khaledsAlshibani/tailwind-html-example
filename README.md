<h1>Tailwind CSS HTML Example</h1>

This is a simple Tailwind CSS project with a simple HTML file. The main purpose of this project was to show a real example of how to use Tailwind CSS with a simple HTML file for beginners.

- [Usage](#usage)
- [How to Create your own Tailwind CSS Project with Simple HTML](#how-to-create-your-own-tailwind-css-project-with-simple-html)
  - [1. Install Tailwind CSS](#1-install-tailwind-css)
  - [2. Create a CSS file](#2-create-a-css-file)
  - [3. Add npm script](#3-add-npm-script)
  - [4. Create the HTML file](#4-create-the-html-file)
  - [5. Run Tailwind CSS](#5-run-tailwind-css)
- [6. Open the HTML file](#6-open-the-html-file)
- [7. Check if Tailwind CSS is working](#7-check-if-tailwind-css-is-working)

## Usage

```bash
npm install
npm run tailwind
```

## How to Create your own Tailwind CSS Project with Simple HTML

### 1. Install Tailwind CSS

```bash
npm install tailwindcss @tailwindcss/cli
```

### 2. Create a CSS file

Create a CSS file (e.g. `css/input.css`) and add the following code:

```css
@import "tailwindcss";
```

### 3. Add npm script

Add the following script to your `package.json` file. The following command will watch for changes in `./css/input.css` and compile it to `./css/style.css`.
```json
"scripts": {
    "tailwind": "npx @tailwindcss/cli -i ./css/input.css -o ./css/style.css --watch"
}
```

So the `css/style.css` will be imported in the `index.html` file.

### 4. Create the HTML file

Create a HTML file and add the following code:

```html
<!DOCTYPE html>
<html>
	<head>
		<meta charset="UTF-8" />
		<meta name="viewport" content="width=device-width, initial-scale=1.0" />
		<link href="./css/style.css" rel="stylesheet" />
	</head>
	<body>
		<h1 class="text-3xl font-bold underline">Hello world!</h1>

        <button type="button" class="focus:outline-none text-white bg-purple-700 hover:bg-purple-800 focus:ring-4 focus:ring-purple-300 font-medium rounded-lg text-sm px-5 py-2.5 mb-2 dark:bg-purple-600 dark:hover:bg-purple-700 dark:focus:ring-purple-900">Purple</button>
	</body>
</html>
```

### 5. Run Tailwind CSS

Run the following command to start the Tailwind CSS compiler:

```bash
npm run tailwind
```

## 6. Open the HTML file

Open the `index.html` file in your browser.

## 7. Check if Tailwind CSS is working

If you see the following screenshot, then Tailwind CSS is working.

<img src="https://i.ibb.co/FLGD7S1f/tw-screenshot.png" alt="Screenshot of Tailwind CSS" >