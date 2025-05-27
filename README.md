# Tailwind CSS Setup Guide

This guide walks you through setting up **Tailwind CSS** in your project using the **Tailwind CLI**. This is the simplest and fastest way to get up and running with Tailwind CSS from scratch.

---

## 📦 Prerequisites

### 1. Install Node.js and npm

First, download and install Node.js from the [official website](https://nodejs.org/). This will also install **npm**, the Node package manager.

You can verify the installation by running:

```bash
node -v
npm -v
```
Project Setup
2. Initialize a New Project
Create a new folder for your project and initialize it with npm:

```bash

mkdir my-tailwind-project
cd my-tailwind-project
npm init -y
```
🌬️ Install Tailwind CSS
3. Install Tailwind CLI
Install tailwindcss and @tailwindcss/cli as development dependencies:

```bash
npm install tailwindcss @tailwindcss/cli
```
📝 Configure Your CSS
4. Create the Input CSS File
Inside your project folder, create a file at src/input.css and add the following:

```css
@import "tailwindcss";
```
🔧 Build CSS with the Tailwind CLI
5. Start the Tailwind Build Process
Run the Tailwind CLI tool to scan your files and build your CSS. Use the --watch flag to automatically rebuild when files change:

```bash
npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch
```
💻 Use Tailwind in HTML
6. Create an HTML File
Create a file named index.html in the src/ directory with the following content:

```html
<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="./output.css" rel="stylesheet">
</head>
<body>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
</body>
</html>
```

