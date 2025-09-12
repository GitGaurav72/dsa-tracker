# Quick Notes - PDF Reader

![Quick Notes Banner](https://via.placeholder.com/800x200/667eea/ffffff?text=Quick+Notes+-+Advanced+PDF+Reader)

Quick Notes is a modern, feature-rich PDF reader built with HTML, CSS, and JavaScript. It offers a beautiful interface with both light and dark themes, advanced navigation features, and usage statistics.

## 🌟 Features

### 📚 PDF Management
- **Square-shaped Book Grid**: Beautiful square layout for PDF thumbnails
- **PDF View Counter**: Tracks views for each individual PDF
- **Quick Access**: One-click access to your PDF collection

### 🎨 Themes & Customization
- **Light/Dark Mode**: Toggle between beautiful light and dark themes
- **Night Sky Effect**: Enjoy a stunning night sky with twinkling stars in dark mode
- **Smooth Animations**: Elegant transitions and hover effects

### 🧭 Navigation & Controls
- **Page Slider**: Jump to any page quickly with the interactive slider
- **Zoom Controls**: Zoom in and out of PDF pages
- **Keyboard Navigation**: Previous/next page buttons
- **Back to Library**: Easy navigation to return to your PDF collection

### 📊 Statistics & Analytics
- **Access Counter**: Tracks unique IP addresses accessing the application
- **Page View Counter**: Counts daily visits to the main page
- **PDF View Tracking**: Records how many times each PDF has been viewed

### 📱 Responsive Design
- **Mobile-Friendly**: Fully responsive design that works on all devices
- **Adaptive Layout**: Adjusts to different screen sizes seamlessly

## 🖼️ Screenshots

### Light Theme
![Light Theme](https://via.placeholder.com/600x400/ffffff/000000?text=Light+Theme+Demo)

### Dark Theme with Night Sky
![Dark Theme](https://via.placeholder.com/600x400/0a0e17/ffffff?text=Dark+Theme+with+Night+Sky)

### PDF Viewer with Controls
![PDF Viewer](https://via.placeholder.com/600x400/2d2d2d/ffffff?text=PDF+Viewer+with+Slider)

### Mobile View
![Mobile View](https://via.placeholder.com/300x500/ffffff/000000?text=Mobile+View)

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- PDF files to view (sample PDFs are included in the demo)

### Installation
1. Download the `quickNote-V0.1.html` file
2. Place it in your desired directory
3. Add your PDF files to the same directory
4. Open the HTML file in your web browser

### Usage
1. **Viewing PDFs**: Click on any PDF thumbnail to open it
2. **Navigating Pages**: Use the slider, arrow buttons, or input field to navigate pages
3. **Zooming**: Use the + and - buttons to zoom in and out
4. **Changing Themes**: Click the moon/sun icon to toggle between light and dark modes
5. **Returning to Library**: Click the "Back to Book List" button to return to the main screen

## 🛠️ Customization

### Adding New PDFs
To add new PDFs to your library:
1. Add the PDF file to the same directory as the HTML file
2. Add a new book item in the HTML:

```html
<div class="book-item" onclick="loadBook('YourPDF.pdf')">
  <div class="book-icon"><i class="fas fa-file-pdf"></i></div>
  <h3 class="book-title">Your PDF Name</h3>
  <div class="book-views"><i class="fas fa-eye"></i> <span id="views-yourpdf">0</span></div>
</div>
```

3. Add the PDF to the viewCounts object in the JavaScript:

```javascript
viewCounts = {
  // ... existing PDFs
  'YourPDF.pdf': 0
}
```

### Modifying Colors and Styles
The application uses CSS variables for easy customization. Modify these variables in the `:root` section:

```css
:root {
  --primary-bg: linear-gradient(135deg, #your-color 0%, #your-color 100%);
  --dark-bg: #your-dark-color;
  /* Add more customizations as needed */
}
```

## 📊 Data Storage

Quick Notes uses localStorage to persist:
- User theme preference
- PDF view counts
- Access counter (simulated IP-based tracking)
- Page view counts

## 🌐 Browser Compatibility

| Browser | Support |
|---------|---------|
| Chrome | ✅ Full support |
| Firefox | ✅ Full support |
| Safari | ✅ Full support |
| Edge | ✅ Full support |
| Internet Explorer | ⚠️ Limited support |

## 📝 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check [issues page](#).

## 🏆 Acknowledgments

- PDF.js library for PDF rendering capabilities
- Font Awesome for the beautiful icons
- Modern CSS techniques for animations and effects

## 📞 Support

If you have any questions or need help with Quick Notes, please open an issue or contact us at support@quicknotes.com.

## 🔄 Version History

- **v0.1** (Current)
  - Initial release
  - Basic PDF viewing functionality
  - Light/dark theme toggle
  - View counters for PDFs

---

**Quick Notes** - Making PDF reading beautiful and efficient.