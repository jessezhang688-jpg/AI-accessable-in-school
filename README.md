# AI Chat Widget for Google Sites

A lightweight, feature-packed, single-file AI chat application designed to embed seamlessly into Google Sites or run as a standalone web app. Built with vanilla HTML, CSS, and JavaScript, it features rich text formatting, math rendering, and customizable AI personas.

## Features

* **Dark & Light Themes:** Toggle seamlessly between dark and light modes with persistent local storage saving.
* **Markdown & Math Support:** Renders rich text formatting (tables, lists, headers, code blocks) using **Marked.js** and scientific math formulas using **KaTeX**.
* **Code Copy Buttons:** Built-in copy buttons atop generated code blocks for easy copy-pasting.
* **Flow-In Text Animation:** Smooth visual block entrance animations for AI responses.
* **Generation Control:** Toggle between **Send** and **Stop** to interrupt output mid-stream.
* **File Attachments:** Attach text/code files to feed context to the AI, featuring slide-up badges and particle destruction effects when removed.
* **Custom AI Persona (System Prompt):** Customize how the AI behaves using a dedicated settings modal. Your custom prompt is saved directly in your browser (`localStorage`).
* **Chat History Export:** Download your active conversation logs into clean `.txt` files with a single click.
* **Quick Escape:** Hit the `Escape` key at any time to instantly redirect out of the page to Google Classroom.

## How It Works

1. **Single-File Architecture:** All HTML, CSS, and JavaScript live within a single `.html` file, making it easy to paste into a Google Sites **Embed** code block.
2. **API Backend:** Sends requests to a Google Apps Script web app endpoint that handles the communication between the UI and the underlying AI model.
3. **Local Storage:** Remembers your preferred visual theme (Light vs. Dark) and your custom AI persona system prompt across browser refreshes.

## How to Use

### 1. Asking Questions
* Type your question into the text box at the bottom and press **Enter** or click **Send**.
* Watch the AI stream its response line by line.

### 2. Customizing the AI Persona
* Click the **Prompt** button in the header bar.
* Enter your instructions (e.g., *"You are a friendly math tutor who explains concepts using simple analogies"*).
* Click **Save Persona**.

### 3. Attaching Files
* Click the **+** button inside the text box to upload a text or code file.
* The AI will read the contents of the attached file along with your message.

### 4. Saving Chat Logs
* Click the **Save** button at the bottom right to download a text file copy of your conversation.

## Tech Stack

* **HTML5 / CSS3 / Vanilla JavaScript**
* **Marked.js**: Markdown parsing
* **KaTeX**: Math formula rendering
* **Google Apps Script**: Proxy endpoint handler
