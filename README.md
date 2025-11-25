# 🔐 Cybersecurity Mind-Map

A **completely free, offline-first mind-map application** for organizing cybersecurity notes, links, files, and knowledge. Deploy instantly on GitHub Pages—no server, no costs, no commands needed.

## ✨ Features

- **📁 Hierarchical Organization** - Create folders and notes in any structure
- **🏷️ Tags & Links** - Categorize and organize URLs to resources
- **💾 Auto-Save** - All data saved to your browser automatically
- **🔒 100% Private** - Data never leaves your device (browser storage only)
- **📤 Export/Import** - Backup your mind-map as JSON anytime
- **📱 Mobile Friendly** - Responsive design works on phones and tablets
- **🌙 Dark Theme** - Easy on the eyes, file-manager inspired UI
- **⚡ Offline Ready** - Works completely offline once loaded
- **🆓 Free Forever** - No costs, no accounts, no tracking

## 🚀 Quick Start

### Option 1: GitHub Pages (Recommended - FREE FOREVER)

1. **Create a GitHub account** at [github.com/signup](https://github.com/signup)
2. **Create new repository** at [github.com/new](https://github.com/new)
   - Name: `cybersecurity-mindmap`
   - Select "Public"
3. **Upload files directly**:
   - Click "Add file" → "Upload files"
   - Upload: `index-static.html`, `mindmap.json`, `.gitignore`
   - Click "Commit changes"
4. **Rename `index-static.html` to `index.html`**:
   - Click the file, click pencil icon, change filename, commit
5. **Enable GitHub Pages**:
   - Go to Settings → Pages
   - Source: "Deploy from a branch"
   - Branch: "main" / Folder: "/" (root)
   - Click Save

**Your app is live at**: `https://YOUR-USERNAME.github.io/cybersecurity-mindmap/`

### Option 2: Local Development (Replit)

1. Open [Replit](https://replit.com) and import this repository
2. The Flask server (`app.py`) runs with full OCR capabilities
3. Access at: `http://localhost:5000`

## 📖 How to Use

### Adding Content
1. **Create Node**: Click "➕ Add Child" to create a new note or folder
2. **Edit**: 
   - Change "Name" to rename
   - Select "Type" (folder or file)
   - Write in "Content / Notes"
3. **Save**: Click "💾 Save Changes"

### Organizing
- **Expand/Collapse**: Click arrows (▶/▼) to expand folders
- **Navigate**: Click any node name in the tree to select it
- **Delete**: Click "🗑️ Delete Node" (deletes node and all children)

### Categorizing
- **Tags**: Add tags like "important", "todo", "research"
- **Links**: Add URLs to cybersecurity resources
- **Delete Items**: Click the "×" button on any tag or link

### Backup & Restore
- **Export**: Click "📥 Export Data" to download a JSON backup
- **Import**: Click "📤 Import Data" to upload a previous backup
- **Location**: Backups are `.json` files on your computer

## 🏗️ Project Structure

```
.
├── index-static.html          # Main app (GitHub Pages version)
├── app.py                     # Flask backend (Replit version)
├── mindmap.json              # Sample data structure
├── .gitignore                # Git settings
├── replit.md                 # Project documentation
└── README.md                 # This file
```

### Two Versions

**`index-static.html` (GitHub Pages)**
- Runs 100% in your browser
- Data stored in localStorage
- No server needed
- Free forever on GitHub Pages
- Works offline

**`app.py` (Replit)**
- Full-featured Flask backend
- Server-side OCR extraction
- File upload processing
- Advanced text extraction
- Requires Python hosting

## 💾 Data Storage

### Where Is My Data Stored?

**GitHub Pages Version (index-static.html)**:
- Stored in your **browser's localStorage**
- Persists across page refreshes
- Cleared only if you clear browser data
- Unique to each browser/device

**Replit Version (app.py)**:
- Stored in `mindmap.json` on the server
- Persists across restarts
- Files stored in `uploads/` folder
- Accessible from any browser/device

### Backup Strategy

1. **Regular Exports**: Click "📥 Export Data" weekly
2. **Store Locally**: Save JSON files on your computer
3. **Cloud Sync**: Upload backups to Google Drive, Dropbox, etc.
4. **Git Backup**: Commit `mindmap.json` to GitHub

## 🔒 Privacy & Security

- ✅ **No tracking** - No analytics, no metrics
- ✅ **No accounts** - No login required
- ✅ **No cloud** - Data never leaves your device (GitHub Pages version)
- ✅ **No ads** - Completely ad-free
- ✅ **Open source** - Code is publicly visible
- ✅ **Encrypted storage** - localStorage is per-domain, isolated

## 🌐 Deployment Comparison

| Feature | GitHub Pages | Replit |
|---------|--------------|--------|
| **Cost** | FREE | FREE (free tier) |
| **Lifetime** | Forever | Indefinite |
| **Requires setup** | No | Yes |
| **OCR extraction** | No | Yes |
| **File uploads** | No | Yes |
| **Works offline** | Yes | No |
| **Multi-device** | Per browser | Yes |

## 🔧 Advanced: Replit Deployment

### Setup
1. Import this repository to [Replit](https://replit.com)
2. Install dependencies: `pip install -r requirements.txt`
3. Run: `python app.py`

### Full Features
- ✅ PDF text extraction (PyPDF2)
- ✅ Image OCR (Tesseract)
- ✅ Word document parsing (python-docx)
- ✅ Excel spreadsheet parsing (openpyxl)
- ✅ CSRF protection
- ✅ Server-side file processing

### Environment Variables
```bash
SESSION_SECRET=your-secret-key-here
```

## 📚 Use Cases

Perfect for:
- 🎓 **Cybersecurity Students** - Organize learning materials
- 🔍 **Security Researchers** - Track research and findings
- 🛡️ **Professionals** - Maintain security reference library
- 📖 **Knowledge Management** - Build personal wiki
- 🔐 **Sensitive Data** - All data stays local (offline-capable)

## ❓ FAQ

**Q: Is my data really private?**
A: Yes. GitHub Pages version stores everything in browser localStorage—nothing is sent to servers.

**Q: Can I use this on my phone?**
A: Yes! It's fully responsive and works on mobile browsers.

**Q: What if I clear browser data?**
A: Your data will be lost. Always keep backups using the "Export Data" button.

**Q: Can I share my mind-map with others?**
A: You can share the GitHub URL, but each person gets their own separate copy. For collaboration, export and share the JSON file.

**Q: Does it cost anything?**
A: No. Completely free on GitHub Pages. No credit card required.

**Q: How much storage do I get?**
A: GitHub Pages: Limited by browser localStorage (~5-10MB)
Replit: Limited by hosting limits

**Q: Can I add files/PDFs?**
A: GitHub Pages version: No file uploads (browser storage only)
Replit version: Yes, full file upload and OCR support

## 🐛 Troubleshooting

**Data not saving?**
- Check browser localStorage is enabled
- Try exporting and re-importing
- Check browser console (F12) for errors

**App not loading?**
- Hard refresh (Ctrl+Shift+R or Cmd+Shift+R)
- Clear browser cache
- Try a different browser

**Lost data?**
- Check if you have an exported JSON backup
- Revert repository to earlier commit if using git

## 📝 License

This project is open source and free to use.

## 🤝 Contributing

Found a bug? Have an idea? Feel free to:
1. Fork this repository
2. Make changes
3. Submit a pull request

## 📞 Support

For questions or issues:
- Check the troubleshooting section above
- Review your browser's developer console (F12)
- Export your data and share the JSON for debugging

---

**Happy organizing! 🎉**

*Built with ❤️ for cybersecurity professionals and students everywhere.*
