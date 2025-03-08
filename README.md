# Welcome to JD Portfolio 👋

![Static Badge](https://img.shields.io/badge/version-v1.1-blue.svg?cacheSeconds=2592000")

> This website is a portfolio built for Jesiah, showcasing his work and providing a clean and interactive user experience with a modern design. The site features a dynamic gallery, filtering, hover effects, and a lightbox for image display

### ✨ Home

You can view the live website soon

### ✍️ Features

- **Responsive Design:** The website is designed to be responsive and work seamlessly across various devices and screen sizes.
- **Image Gallery:** A dynamic image gallery powered by JavaScript, allowing users to filter and view images by category.
- **Lightbox:** A lightbox feature for enlarged image viewing.
- **Floating Tab Menu:** A user-friendly floating tab menu for easy navigation to bio and contact information.
- **Filter Navigation:** Filter gallery images by category and change gallery display columns.
- **Tailwind CSS:** Utilizes Tailwind CSS for rapid UI development.
- **JSON Data:** Image data is loaded from a JSON file, making it easy to update the gallery.
- **Performance Optimization:** Includes lazy loading for images and optimized JavaScript for smooth user experience.

### 🧑‍💻 Technologies Used

- HTML
- CSS (Tailwind CSS)
- JavaScript
- JSON

### 🧱 Project Structure

```
root/
├─ bio.html
├─ contact.html
├─ css
│  └─ style.css
├─ font
│  └─ wakerobin-regular.otf
├─ img
│  ├─ client
│  │  ├─ client (1).webp
│  ├─ events
│  │  ├─ events (1).webp
│  ├─ gallery.json
│  ├─ icons
│  │  ├─ menu-close.webp
│  │  └─ menu-open.webp
│  ├─ jes-des-media-logo.webp
│  ├─ jesiah-desaine.webp
│  └─ restaurant
│     ├─ restaurant (1).webp
├─ index.html
├─ js
│  ├─ filter.js
│  ├─ gallery.js
│  └─ generateImages.js
├─ netlify
│  └─ functions
│     └─ fetchImages.js
├─ package-lock.json
├─ package.json
└─ README.md
```

> [!IMPORTANT]
This application's image gallery is dynamically populated from a [Supabase database](https://github.com/supabase/supabase-js). The database stores both image files and their associated categories.

**Local Development (Without Database)**

1.  **Verify and Install Node.js:**
    * **Check Installation:** Open your terminal (or command prompt on Windows) and enter `node -v`.
    * If a version number appears, Node.js is installed.
    * **Installation (if necessary):**
        * Navigate to the official Node.js website: [nodejs.org](https://nodejs.org/).
        * Download the recommended LTS (Long Term Support) version.
        * Execute the downloaded installer and complete the setup process.
2.  Organize your image files and categories into the appropriate subdirectories within the `img` folder.
3.  Execute the `generateImages.js` script by running `node generateImages.js` in your terminal. This script will create the `gallery.json` file within the `img` directory.
4.  Update the `gallery.js` file to load image data from the generated `gallery.json` file. Replace the database fetch logic with:

```javascript
fetch("img/gallery.json")
  .then(response => response.json())
  .then(images => {
    // Implement your image rendering and application logic here.
  })
  .catch(error => {
    console.error("Error loading image data:", error);
  });
```

## Developer

👤 **Kevan**

- Website: [My Portfolio](https://xkevan19.github.io/PortfolioV1.2)
- Github: [@xkevan19](https://github.com/xkevan19)
- LinkedIn: [@https:\/\/www.linkedin.com\/in\/kevansuchit\/](https://linkedin.com/in/https://www.linkedin.com/in/kevansuchit/)

## 🤝 Contributing

Contributions, issues and feature requests are welcome! Feel free to check [issues page](https://github.com/xkevan19/JD-Portfolio/issues).
