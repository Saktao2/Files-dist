# Files-Dist: Webpack Configuration  

This project demonstrates how to use Webpack to bundle and optimize a simple web application.  

---

## 📂 File Structure  

files-dist/ 
├── dist/ # Output folder (created after build)
├── node_modules/ # Installed dependencies
├── src/ # Source files
│ ├── index.html # Main HTML file
│ ├── style.css # Main CSS file
│ └── script.js # Main JavaScript file
├── package.json # Project configuration and scripts
├── webpack.config.js # Webpack configuration
└── README.md # Project documentation

---

## 🚀 Features: What It Does  

- **JavaScript Bundling**:  
  Takes the main JavaScript file (`script.js`) specified in the `entry` property and combines it with any dependencies into a single, optimized `bundle.js` file. This reduces the number of requests made by the browser.  

- **CSS Processing and Injection**:  
  Processes all CSS files using `css-loader` (to interpret `@import` and `url()`) and `style-loader` (to inject the CSS into the DOM). This ensures your CSS is dynamically applied to the HTML at runtime without needing separate CSS files.  

- **HTML Optimization**:  
  The `HtmlWebpackPlugin` takes your `index.html` file as a template, injects references to the bundled JavaScript file (`bundle.js`), and minifies the HTML by:  
  - Removing comments.  
  - Collapsing unnecessary whitespace.  

- **Clean Output Directory**:  
  The `clean: true` option in the `output` configuration ensures that the `dist` folder is cleared before each build, removing old or unused files.  

- **Production-Ready Output**:  
  By setting `mode: 'production'`, Webpack automatically applies optimizations, including:  
  - Minification of JavaScript.  
  - Tree-shaking to remove unused code.  
  - Better performance and smaller bundle size.  



---

## 🔧 Setup How to use it

### Prerequisites  

Make sure you have the following installed:  
- [Node.js](https://nodejs.org/) (v16 or higher recommended)  
- [npm](https://www.npmjs.com/)  

### Installation  

1. Clone this repository or download the files.  
2. Open a terminal and navigate to the project folder.  
3. Install dependencies:  
   ```bash
   npm install

---

### 🛠️ Usage

Build the Project:

To bundle and optimize the files, run npx webpack

This will create the dist/ folder


### 📝 License

This project is licensed under the MIT License.

Credits to: https://webpack.js.org
