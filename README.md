# 🗺️ Mind Map Viewer

A lightweight, interactive, and beautifully-styled browser-based viewer for FreeMind (.mm) mind map files. This tool parses .mm files and renders them as dynamic, collapsible trees using D3.js, with a modern UI built in Tailwind CSS.

## ✨ Features

This isn't just a simple viewer; it's packed with features for a great user experience:

### 📁 File Loading
- **Drag & Drop**: Simply drop your .mm file anywhere on the page to load it
- **File Upload**: Use the dedicated upload button to select a file

### 🎨 Interactive Visualization (D3.js)
- **Collapsible Nodes**: Click any node to expand or collapse its children
- **Smooth Transitions**: All expanding, collapsing, and layout changes are smoothly animated
- **Tooltips**: Hover over a node to see its full name, depth, and child count
- **Node Selection**: Ctrl/Cmd + Click to select a specific node

### 📐 Dual Layouts
- **Horizontal (Mind Map)**: A classic mind map layout, spreading from left to right
- **Vertical (Org Chart)**: A top-down organization chart layout

### 🔍 Pan & Zoom
- **Mouse/Trackpad**: Use your mouse wheel or trackpad to zoom and click-and-drag to pan
- **UI Controls**: Dedicated buttons for Zoom In (+), Zoom Out (-), and a vertical slider
- **Fit to Screen**: A one-click button (A) to perfectly center and fit the entire map to your viewport

### 🎨 Theming & Styling
- **3-Mode Theme Toggle**: Switch instantly between Light, Dark, and AMOLED (OLED black) modes
- **Node Color Picker**: Choose a custom color and apply it to all nodes in the mind map
- **Reset Colors**: A button to clear custom colors and revert to the map's original (or default) styling

### 🔎 Search
- **Live Search**: A debounced search bar that highlights nodes matching your query in real-time
- **Dimming**: Non-matching nodes are dimmed for clear focus

### 💾 Export Options
- **Export as SVG**: Download a high-quality, scalable vector graphic of the current view
- **Export as PNG**: Download a high-resolution PNG image (with the correct background color!)
- **Export as JSON**: Get the parsed JSON hierarchy, perfect for developers
- **Export as .MM**: Re-export the mind map as a .mm file, preserving any color changes

### 🖥️ UI & Other Features
- **Fullscreen Mode**: View your mind map without distractions
- **State Persistence**: The app uses localStorage to remember your last-loaded mind map, including its collapsed state and custom colors
- **Responsive Design**: The UI works great on both desktop and mobile devices
- **Error Handling**: Displays user-friendly toast messages for errors (e.g., invalid file type)

## ⌨️ Keyboard Shortcuts

The viewer is fully navigable using your keyboard:

| Key | Action |
|-----|--------|
| `Arrow Keys` | Navigate between visible nodes (up, down, left, right) |
| `Enter` / `Space` | Toggle (expand/collapse) the currently selected node |
| `Escape` | Clear the current node selection |
| `E` | Expand/Collapse the entire subtree of the selected node |
| `A` | All-in-one fit: Fits the map to the screen |
| `F` | Toggle Fullscreen mode |
| `T` | Toggle Theme (Light → Dark → AMOLED) |
| `+` / `=` | Zoom In |
| `-` | Zoom Out |

## 🛠️ Technologies Used

- **D3.js (v7)**: The core engine for data visualization, handling the tree hierarchy, zoom/pan, and SVG rendering
- **Tailwind CSS**: Used for the entire UI, including the responsive layout, theme-switching, and all component styling
- **Plain JavaScript (ES6+)**: All application logic, including the .mm XML parser, state management, and event handling, is written in modern, dependency-free JavaScript
- **Google Fonts**: Uses the Inter font for clean, modern, readable text
- **Material Symbols**: Provides all the icons used in the UI

## 🚀 How to Use

Since this is a single-file, client-side application, getting started is simple:

1. **Open the File**: Just open the `index.html` file in any modern web browser (like Chrome, Firefox, Safari, or Edge)

2. **Load a Map**:
   - Drag and drop a `.mm` file (from FreeMind or a compatible app) onto the browser window
   - ...or click the Upload icon and select your file

3. **Explore**:
   - Click nodes to explore the map
   - Use the controls in the header to search, change layouts, and customize the look
   - Use the zoom controls on the right to get the perfect view

## 📄 License

This project is open-source and available under the MIT License.
