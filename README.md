# Urban Observation Tool

## Overview

The Urban Observation Tool is a web-based interface designed for conducting site visits and observations in urban environments. It provides tools for managing checklists, adding notes with photos and locations, organizing categories, and assigning staff. This tool appears to be geared toward urban planners, field researchers, or inspectors who need to document observations systematically.

The provided HTML file (`urban_observation_staff (1).html`) represents the core user interface, including modals for editing, adding items, and managing content. It uses Font Awesome icons for visual elements and supports basic interactions like photo capture and note-taking.

**Note**: This is a static HTML structure. Full functionality (e.g., photo uploading, location detection, or dynamic updates) would require additional JavaScript, CSS, and possibly a backend server. The HTML serves as a prototype or template.

## Features

- **Observation Checklist**: A central view for listing and managing observation items.
- **Staff Library**: A modal for selecting and managing staff members, with search functionality.
- **Add Category**: Create new categories with customizable names, staff assignments, and icons (e.g., tree, road, building).
- **Add Note**: 
  - Capture or upload photos (via camera or gallery).
  - Add textual content.
  - Automatically record location coordinates with photos.
- **Item Management**:
  - Edit item names.
  - Add new items at specific positions (top, after current, bottom).
  - Move items up/down.
  - Delete items.
- **Photo Handling**: Supports taking photos or selecting from a gallery, with placeholders for no photos.
- **Icons and UI Elements**: Uses Font Awesome for icons like tree (fa-tree), road (fa-road), etc.

## Requirements

- A modern web browser (e.g., Chrome, Firefox, Safari).
- Font Awesome library (include via CDN: `<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">` for icons to render properly).
- Optional: JavaScript framework (e.g., jQuery or vanilla JS) for handling modals, form submissions, and dynamic features like photo capture (using `navigator.mediaDevices` API).

## Installation

1. Download or copy the HTML file (`urban_observation_staff (1).html`).
2. Include Font Awesome in the `<head>` section if not already present:
   ```
   <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
   ```
3. Open the file in a web browser to view the interface.

No build tools or dependencies are required for the basic static view.

## Usage

1. **Open the Tool**: Load the HTML file in your browser.
2. **Navigate Sections**:
   - Use the "Staff Library" button to access staff selection.
   - Click "Add Category" to create new observation categories.
   - In the "Observation Checklist", interact with items using edit, add, move, or delete options.
3. **Add a Note**:
   - Click "Add Note".
   - Take a photo or upload from gallery.
   - Enter note content.
   - Location is auto-recorded (requires browser geolocation permissions).
   - Save or delete as needed.
4. **Customization**:
   - Modals like "Edit Item" or "Add New Item" allow inline changes.
   - Categories can be assigned to staff and given thematic icons.

For production use, integrate with JavaScript to handle events (e.g., modal toggles via `data-toggle` attributes if using Bootstrap) and persist data (e.g., via localStorage or a database).

## Limitations

- Static HTML only; no backend for data storage or user authentication.
- Photo and location features rely on browser APIs and may not work in all environments (e.g., non-HTTPS sites for camera access).
- No CSS provided in the snippet; apply custom styles for better visuals.
- Geolocation requires user permission and device support.

## Contributing

This is a basic prototype. Contributions could include:
- Adding CSS for responsive design.
- Implementing JavaScript for interactivity.
- Integrating with a framework like React or Vue for a full app.

Fork the repository (if hosted) and submit pull requests.

## License

© 2023 Urban Observation Tool. All rights reserved. This tool is provided as-is for educational or demonstration purposes. For commercial use, contact the copyright holder.
