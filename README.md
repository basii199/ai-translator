
# iTranslate

iTranslate is a modern and interactive AI-powered web application that allows users to **detect languages**, **translate text**, and **summarize messages** using an intuitive chat-like interface.

## Features

- 🔍 **Language Detection**: Detects the language of the input text with a confidence score.
- 🌐 **Translation**: Translates text to a selected target language.
- 📄 **Summarization**: Provides a concise summary of long-form input text.
- ⚡ Smooth UI with real-time feedback using loaders and type animations.
- 🎯 Automatic action suggestions for short and long messages.

## Technologies Used

- **React** with hooks
- **JavaScript** and modern ES6+ features
- **TailwindCSS** for responsive UI
- **react-type-animation** and **react-spinners** for dynamic UI feedback

## Components Overview

### 1. `App.jsx`
- Main entry point managing application-wide state (message, action, AI readiness).
- Renders `ErrorHeader`, `ChatArea`, `InputArea`, and `Footer`.

### 2. `InputArea.jsx`
- Textarea input for user messages.
- Dynamically resizes based on input length.
- Action buttons to select: Detect, Translate, Summarize.
- Submit button triggers message processing.

### 3. `ChatArea.jsx`
- Displays messages and AI responses.
- Handles dynamic rendering based on selected actions.
- Displays loading animations during processing.

### 4. Utility Functions
- `summarize`, `detectLanguage`, `translateMessage`: Interface with AI APIs.
- `renderMessage`, `renderResponse`: DOM manipulation to render user and AI messages.
- `TranslateOptions`: A dropdown component for selecting translation targets.

## Getting Started

1. Clone the repo
```bash
git clone https://github.com/basii199/ai-translator.git
cd iTranslate
```

2. Install dependencies
```bash
npm install
```

3. Run the app
```bash
npm run dev
```

> Make sure AI capabilities (`translator`, `summarizer`, `languageDetector`) are available and properly configured in your environment.

## Folder Structure

```
components/
├── ChatArea.jsx
├── ErrorHeader.jsx
├── Footer.jsx
├── InputArea.jsx
├── TranslateOptions.jsx
utilities/
├── detectLanguage.js
├── summarize.js
├── renderMessage.js
├── renderResponse.js
├── translateMessage.js
App.jsx
```

## License

This project is licensed under the MIT License.
