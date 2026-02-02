//installation guide by chatgpt
# Natours — Installation Guide

This guide helps a new developer clone the repository and set up the project locally.

---

## Prerequisites

Make sure you have installed:

- **Node.js** (v16+ recommended)  
- **npm** (comes with Node.js)  
- Optional: Git (for cloning)

---

## 1. Clone the repository

```bash
git clone https://github.com/prahans/Natours.git
cd Natours

2. Install dependencies

npm install
This installs the required dev dependency sass for compiling SCSS.

3. Compile Sass to CSS
One-time compile
npm run compile:sass


This will compile sass/main.scss into css/main.css.

Automatic watch mode
npm run watch:sass


Watches for changes in SCSS files

Automatically updates main.css whenever you save

4. Open the project

Open index.html in your browser

Or use a live server (like VS Code Live Server extension) for hot-reloading

5. Notes for Developers

Do not edit main.css manually — always edit SCSS files in sass/

Compiled CSS (main.css) and .map files are ignored in Git (.gitignore)

If cloning the repo fresh, always run npm run compile:sass first

6. Optional: Contributing

Fork the repository

Create a feature branch: git checkout -b feature/your-feature

Make changes and commit: git commit -m "Add your feature"

Push to your branch: git push origin feature/your-feature

Open a Pull Request

Tip

Always work with SCSS source files; use the npm scripts to compile for development or production.

//written by anurag
Natours
lean about atomic design from this youtube video -> https://youtu.be/Yi-A20x2dcA?si=FQaVaMYF7OT_T4kq

BEM -> Block Element Modifier 
BLOCK : standalone component that is meaningful on its own.
ELEMENT : part of a block that has no standalone meaning.
MODIFIER : a different version of a block or element.

.block {}
.block__element {}
.block__element--modifier {}

* ARCHITECT
THE 7-1 PATTERN
7 different folders for partial Sass files, and
1 main Sass file to import all others files into a compiled CSS stylesheet.

THE 7 FOLDERS
.base/
.components/
.layout/
.pages/
.themes/
.abstracts/
.vendors/

we can use :not sudo class 