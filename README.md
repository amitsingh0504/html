
This README includes:
- Project overview
- Feature list
- Getting started instructions
- Multiple ways to run locally
- Project structure
- Usage guide
- Testing instructions
- Browser compatibility notes
- Technologies used
- Customization tips

html/
├── index.html      # Main HTML file with all examples
├── style.css       # Stylesheet with responsive design
└── README.md      # This file

# HTML & HTML5 APIs Playground

A comprehensive, interactive playground for learning and experimenting with HTML tags and HTML5 APIs. This project demonstrates modern web development techniques with clean, responsive design and hands-on examples.

## 🎯 Features

### HTML Elements Covered
- **Text Formatting**: Headings, paragraphs, strong, em, mark, code, quotes, and more
- **Semantic HTML5**: header, nav, main, section, article, footer, details, summary
- **Lists**: Unordered, ordered, and description lists with nesting
- **Tables**: Complete table structure with thead, tbody, tfoot, and captions
- **Media Elements**: Images, video, audio, SVG, and Canvas
- **Forms**: All input types** including text, email, password, number, date, time, color, file, range, checkbox, radio, select, datalist, and textarea

### HTML5 APIs Demonstrated
- **Geolocation API**: Get user's current location
- **Local Storage API**: Store and retrieve data persistently
- **Session Storage API**: Store data for the current session
- **Drag and Drop API**: Interactive drag and drop functionality
- **Web Workers**: Background processing without blocking the UI
- **History API**: Manipulate browser history programmatically
- **Fullscreen API**: Toggle fullscreen mode
- **Page Visibility API**: Detect when page is visible or hidden
- **Clipboard API**: Copy text to clipboard
- **Fetch API**: Make HTTP requests (may require local server)

### Design Features
- ✨ Modern, clean UI with smooth transitions
- 🌙 Dark mode toggle
- 📱 Fully responsive design (mobile, tablet, desktop)
- 🎨 Beautiful gradient effects and hover animations
- ♿ Accessible form labels and semantic HTML

## 🚀 Getting Started

### Quick Start

1. **Clone or download this repository**
   
   git clone <repository-url>
   cd html
   2. **Open the HTML file**
   - Simply double-click `index.html` to open in your default browser
   - Or right-click and choose "Open with" your preferred browser

### Using a Local Server (Recommended)

Some APIs (like Fetch) work better with a local server. Here are several options:

#### Option 1: Python HTTP Serversh
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000Then open: `http://localhost:8000`

#### Option 2: Node.js HTTP Server
npx http-server -p 8000Then open: `http://localhost:8000`

#### Option 3: VS Code Live Server
1. Install the "Live Server" extension in VS Code
2. Right-click `index.html` → "Open with Live Server"

#### Option 4: PHP Built-in Server
php -S localhost:8000## 📁 Project Structure
