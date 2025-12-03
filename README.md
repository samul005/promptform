# PromptManager Pro - Llama Edition

A modern, AI-powered prompt management application with intelligent auto-fill capabilities using Meta's Llama 3.3 70B model.

## 🚀 Features

### Core Functionality
- **Prompt Management**: Create, edit, delete, and organize prompts with ease
- **AI Auto-Fill**: Automatically generate titles and descriptions from prompt content using Llama 3.3 70B
- **Bulk Import/Export**: Support for CSV and JSON formats with merge or replace options
- **Drag & Drop**: Easy file upload with drag-and-drop interface
- **Search**: Real-time search across all prompts
- **Dual View Modes**: Switch between table and grid layouts
- **Pagination**: Efficient handling of large prompt collections (50 items per page)

### Advanced Features
- **Image Support**: Upload and embed images with prompts (Base64 encoding)
- **Categorization**: Organize prompts with categories and sub-categories
- **Tags**: Mark prompts as "New" or "Trending"
- **Local Storage**: All data persists locally in your browser
- **Copy to Clipboard**: Quick copy functionality for prompt content
- **Toast Notifications**: Real-time feedback for all actions

## 🎨 User Interface

- **Modern Design**: Built with Tailwind CSS for a clean, professional look
- **Responsive Layout**: Works seamlessly on desktop and mobile devices
- **Custom Icons**: FontAwesome 6.4.0 integration
- **Smooth Animations**: Fade-in effects and shimmer loading states
- **Custom Scrollbars**: Enhanced visual experience

## 🛠️ Technology Stack

- **Frontend Framework**: React 18 (via CDN)
- **Styling**: Tailwind CSS
- **Icons**: FontAwesome 6.4.0
- **Build Tool**: Babel Standalone (in-browser JSX compilation)
- **AI Integration**: OpenRouter API with Llama 3.3 70B
- **Storage**: Browser LocalStorage API

## 📋 Prerequisites

- Modern web browser (Chrome, Firefox, Safari, Edge)
- OpenRouter API key (optional - for AI auto-fill features)

## 🚀 Getting Started

### Installation

1. Clone the repository:
```bash
git clone https://github.com/samul005/promptform.git
cd promptform
```

2. Open `index.html` in your web browser:
```bash
# On macOS
open index.html

# On Linux
xdg-open index.html

# On Windows
start index.html
```

Or use a local server:
```bash
# Using Python 3
python -m http.server 8000

# Using Node.js http-server
npx http-server -p 8000
```

Then navigate to `http://localhost:8000` in your browser.

### Configuration

#### Setting Up AI Auto-Fill

1. Click the settings icon (⚙️) in the header
2. Enter your OpenRouter API key
3. Click "Save Settings"

The application comes with a default API key, but you can replace it with your own for production use.

## 📖 Usage Guide

### Creating a New Prompt

1. Click the "New Prompt" button in the header
2. Enter the prompt content (required)
3. Optionally click "Auto-Fill Details" to generate title and description using AI
4. Add optional metadata:
   - Category and Sub-category
   - Image asset
   - Mark as New/Trending
5. Click "Save Prompt"

### Importing Data

1. Click the "Import" button
2. Choose import mode:
   - **Merge**: Combine with existing data (duplicates overwritten)
   - **Replace All**: Delete existing data and import new
3. Import via:
   - Drag & drop CSV files
   - Browse and select files
   - Paste CSV or JSON data directly

#### CSV Format
```csv
PROMPT_TITLE,PROMPT_CONTENT,DESCRIPTION,IMAGE_URL,CATEGORY,SUB_CATEGORY,MARK_AS_NEW,MARK_AS_TRENDING
"Example Title","Example content","Example description","","General","","TRUE","FALSE"
```

#### JSON Format
```json
[
  {
    "PROMPT_TITLE": "Example Title",
    "PROMPT_CONTENT": "Example content",
    "DESCRIPTION": "Example description",
    "IMAGE_URL": "",
    "CATEGORY": "General",
    "SUB_CATEGORY": "",
    "MARK_AS_NEW": false,
    "MARK_AS_TRENDING": false
  }
]
```

### Exporting Data

1. Click the "Export" button
2. Choose format:
   - **CSV**: Compatible with Excel and Google Sheets
   - **JSON**: For programmatic use or backup

### Managing Prompts

- **Edit**: Click the edit icon (✏️) on any prompt
- **Delete**: Click the trash icon (🗑️) and confirm
- **Copy**: Click the copy icon (📋) to copy prompt content to clipboard
- **Search**: Use the search bar to filter prompts by title or content
- **View Modes**: Toggle between table and grid views

## 🗂️ Data Storage

All data is stored locally in your browser using LocalStorage:
- **Prompts**: Stored under `pg_prompts_llama_v2`
- **Settings**: Stored under `pg_settings_llama_v1`

**Important**: Clearing browser data will delete all prompts. Use export functionality for backups.

## 🔐 Privacy & Security

- All data is stored locally in your browser
- No server-side storage or tracking
- API calls only made to OpenRouter when using AI features
- API key stored locally in browser

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

### Development Guidelines

1. Maintain the existing code style
2. Test thoroughly before submitting
3. Keep the single-file architecture
4. Ensure responsive design compatibility

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

Copyright (c) 2025 samuel

## 🙏 Acknowledgments

- Meta for Llama 3.3 70B model
- OpenRouter for API infrastructure
- React, Tailwind CSS, and FontAwesome teams

## 📞 Support

For issues, questions, or contributions, please visit the [GitHub repository](https://github.com/samul005/promptform).

## 🔄 Version History

- **v2**: Updated favicon and storage keys
- **v1**: Initial release with Llama 3.3 70B integration

---

Built with ❤️ using React and Tailwind CSS
