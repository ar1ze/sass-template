# Sass & Webpack Project Starter

This is a modern front-end project starter template, featuring a scalable 7-1 Sass architecture and using Webpack to bundle all assets (JavaScript, SCSS, images, fonts) for development and production.

---

## Features 🚀

  * **Webpack 5:** Bundles all your JavaScript and dependencies into a single file.
  * **Sass Loader:** Compiles your SCSS to CSS and injects it directly into the DOM.
  * **Dev Server:** A live-reloading development server (`webpack-dev-server`) for a smooth workflow.
  * **Asset Handling:** Properly handles images, fonts, and other assets for the final build.
  * **Scalable Sass Architecture:** Organized folders for variables, base styles, components, and layouts.

---

## Getting Started

Follow these steps to get the project up and running on your local machine.

1.  **Clone the repository**

    ```bash
    git clone <your-repository-url>
    ```

2.  **Navigate to the project directory**

    ```bash
    cd <project-name>
    ```

3.  **Install dependencies**

    ```bash
    npm install
    ```

---

## Available Scripts

Once the dependencies are installed, you can use the following commands:

  * **`npm start`**

      * Starts the development server with live reloading at `http://localhost:8080`.
      * The server watches for changes in your `src` files and automatically updates the browser.

  * **`npm run build`**

      * Creates a production-ready build of your project in the `dist` folder.
      * This bundle is optimized and ready to be deployed to a web server.

---

## Sass Architecture

The `scss` folder is structured to keep styles organized and maintainable. It follows a methodology similar to the 7-1 pattern.

  * **`abstracts/`**: Holds Sass tools and helpers. Contains variables, functions, and mixins. No direct CSS output.
  * **`base/`**: Contains boilerplate code for the project, including resets, typographic rules, and global styles.
  * **`components/`**: Contains styles for reusable UI components. Each file represents a specific component.
      * `_button.scss`: Styles for button elements.
  * **`layouts/`**: Contains styles for major parts of the site's layout.
      * `_header.scss`: Styles for the site header.
      * `_sidebar.scss`: Styles for the navigation sidebar.
      * `_main.scss`: Styles for the main content area.
  * **`main.scss`**: The main entry point that imports all other Sass partials in the correct order.

---

## Project Structure

```
.
├── dist/             # Bundled output (auto-generated)
├── src/              # Your source code
│   ├── assets/       # Images, fonts, etc.
│   ├── index.js      # Main JavaScript entry point
│   ├── scss/         # Sass files
│   │   ├── abstracts/
│   │   ├── base/
│   │   ├── components/
│   │   │   └── _button.scss
│   │   ├── layouts/
│   │   │   ├── _header.scss
│   │   │   ├── _main.scss
│   │   │   └── _sidebar.scss
│   │   └── main.scss
│   └── template.html # HTML template file
│
├── package.json
└── webpack.config.js
```

---

## Useful Links & Acknowledgements

  * [Sass Documentation](https://sass-lang.com/documentation)
  * [Webpack Documentation](https://webpack.js.org/)
  * [Sass Guidelines](https://sass-guidelin.es/)

The Sass architecture was inspired by the [technoph1le/sass-template](https://github.com/technoph1le/sass-template) project.