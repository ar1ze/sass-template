# Sass & Webpack Project Starter

A front-end starter template using the 7-1 Sass architecture and Webpack for asset management.

## 🚀 Quick Start

1.  **Create Repository:** Click `Use this template` to create your new repository.
2.  **Clone & Install:**
    ```sh
    git clone https://github.com/your-username/your-repo-name.git
    cd your-repo-name
    npm install
    ```
3.  **Run Development Server:**
    ```sh
    npm start
    ```
    Your site is now running at `http://localhost:8080` with live reload.

-----

## 🛠️ Available Scripts

| Command | Description |
| :--- | :--- |
| `npm start` | Starts the dev server at `localhost:8080` with live reload. |
| `npm run build` | Creates an optimized production build in the `dist` folder. |
| `npm run deploy:init` | **(One-time setup)** Creates the `gh-pages` branch. |
| `npm run deploy` | Deploys the `dist` folder contents to the `gh-pages` branch. |

-----

## 🚀 Deployment to GitHub Pages

### 1\. First-Time Setup

1.  Initialize the deployment branch:
    ```sh
    npm run deploy:init
    ```
2.  In your GitHub repository, go to **Settings \> Pages**.
3.  Set the **Source** to **Branch: `gh-pages`** and **Folder: \`/ (root)**. Save.

Your site will be live at `https://your-username.github.io/your-repo-name/`

### 2\. Deploying Updates

After you `git push` changes to your `main` branch, run:

```sh
npm run deploy
```

This script automatically builds your project and pushes the production-ready `dist` folder contents to the `gh-pages` branch.

-----

## 📁 Project Structure

This project uses the **7-1 Sass pattern**.

  * `public/`: Static assets (favicons, etc.) copied directly to `dist`.
  * `src/`: Your main source code.
      * `assets/`: Fonts, images, and other static assets.
      * `scss/`: All Sass files, organized by the 7-1 pattern (abstracts, base, components, layouts, pages).
      * `index.js`: Main JavaScript entry point.
      * `template.html`: The main HTML file template.
      * `utils/`: JavaScript utility functions.
  * `dist/`: The auto-generated production build folder (git-ignored).

-----

## 📚 Useful Links

  * [Sass Documentation](https://sass-lang.com/documentation)
  * [Webpack Documentation](https://webpack.js.org/concepts/)
  * [Sass Guidelines](https://sass-guidelin.es/)
  * Architecture inspired by [technoph1le/sass-template](https://www.google.com/search?q=https://github.com/technoph1le/sass-template).