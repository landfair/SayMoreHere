# Say More Here - Chrome Extension

A Chrome extension version of the Writing Teachers Comment Bank application. This tool helps writing teachers manage and organize feedback comments for grading assignments.

## Features

- Create and manage multiple comment banks for different assignments
- Add, edit, and organize feedback comments
- Tag comments for easy categorization
- Copy selected comments to clipboard
- Upload and download comment banks
- Filter comments by tags
- Persistent storage using Chrome's storage API

## Installation

### Step 1: Prepare the Icons (Optional but Recommended)

1. Navigate to the `icons` folder
2. Follow the instructions in `icons/README.md` to generate icon files
3. Alternatively, you can skip this step and Chrome will use default icons

### Step 2: Load the Extension in Chrome

1. Open Chrome and navigate to `chrome://extensions/`
2. Enable "Developer mode" using the toggle in the top right corner
3. Click "Load unpacked"
4. Select the `chrome-extension` folder from your file system
5. The extension should now appear in your extensions list

### Step 3: Use the Extension

1. Click the extension icon in your Chrome toolbar (you may need to pin it first)
2. The popup will open showing the Comment Bank interface
3. Start creating comment banks and adding feedback comments

## Files Structure

```
chrome-extension/
├── manifest.json       # Extension configuration
├── popup.html         # Extension popup UI
├── popup.css          # Styles for the extension
├── popup.js           # JavaScript logic
├── icons/             # Extension icons
│   ├── icon.svg       # SVG source for icons
│   └── README.md      # Instructions for generating icons
└── README.md          # This file
```

## Usage Tips

- **Creating Comment Banks**: Click "+ Add Comment Bank" to create a new bank for an assignment
- **Adding Comments**: Open a comment bank and click "+ Add Comment" to add feedback
- **Tagging**: Use the "🏷️ Manage Tags" button to create custom tags for organizing comments
- **Copying**: Select multiple comments with checkboxes and click "📋 Copy Selected" to copy to clipboard
- **Filtering**: Use the tag filter bar to view comments with specific tags
- **Backup**: Use "Download Comment Bank" from the Options menu to backup your data

## Data Storage

All data is stored locally using Chrome's `chrome.storage.local` API. Your comment banks will persist across browser sessions and will only be accessible from your Chrome browser.

## Troubleshooting

### Extension doesn't load
- Make sure you selected the correct folder containing `manifest.json`
- Check that all required files are present
- Look for errors in the Chrome Extensions page

### Popup doesn't display correctly
- Clear your browser cache
- Reload the extension from the Extensions page
- Check the browser console for JavaScript errors

### Data isn't saving
- Ensure the extension has storage permissions (should be automatic)
- Check Chrome's storage quota hasn't been exceeded

## Development

To modify the extension:

1. Make changes to the source files
2. Go to `chrome://extensions/`
3. Click the reload icon on the extension card
4. Test your changes

## Support

For issues, questions, or feature requests, please visit the project repository.

## License

This extension is part of the Say More Here project.
