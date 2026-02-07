# Pragma Education Website

## Project Structure

The project is organized as follows:

```
pragmaeducation.com/
├── assets/
│   ├── css/                # Custom and template CSS files
│   │   ├── custom.css
│   │   └── style.css
│   ├── js/                 # Custom and template JS files
│   │   ├── custom.js
│   │   └── main.js
│   ├── img/                # Images
│   ├── new-img/            # Newer images (logo, favicon)
│   └── vendor/             # Third-party libraries
│       ├── aos/
│       ├── bootstrap/      # Bootstrap 5
│       ├── bootstrap-icons/
│       ├── boxicons/
│       ├── swiper/
│       └── ...
├── index.html              # Main landing page
└── README.md               # This file
```

## Setup Instructions

### Prerequisites
- A web browser (Chrome, Firefox, Edge, etc.)
- Internet connection (for jQuery CDN and Google Fonts)
- A local web server (optional but recommended)

### Running Locally

You can open `index.html` directly in your browser, but for the best experience (especially with some JS features), use a local server.

**Using Python:**
1. Open a terminal in this directory.
2. Run: `python -m http.server 8000`
3. Open `http://localhost:8000` in your browser.

**Using Node.js (npx):**
1. Open a terminal in this directory.
2. Run: `npx serve`
3. Open the URL shown in the terminal.

## Deployment Instructions

1. **Upload**: Upload the entire contents of the `pragmaeducation.com` folder to your web server's public directory (e.g., `public_html`).
2. **Dependencies**: Ensure the server allows outgoing connections if you are using CDNs, or the user's browser has internet access.
3. **Paths**: The `index.html` has been configured with relative paths for assets, so it should work in any subdirectory.

## Changes Made
- Updated absolute paths (e.g., `https://pragmaeducation.com/assets/...`) to relative paths (`assets/...`).
- Consolidated Bootstrap references to use the local Bootstrap 5 files.
- Removed redundant Bootstrap 4 and 5 CDN references.
- Fixed HTML structure (moved scripts inside `<body>`).
- Preserved jQuery CDN reference as it is required by `custom.js`.
