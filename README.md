# � Steps Counter App

A simple, interactive steps counter application built with vanilla JavaScript as part of the Scrimba Frontend Developer Path. Track your daily steps and save your progress with this beginner-friendly web app.

## 🌐 Live Demo

**🚀 [View Live Website](https://step-counter.netlify.app/)** - Experience A simple, interactive steps counter application

![Steps Counter Preview](image.png)

## ✨ Features

- **Real-time Counter**: Increment your step count with a single click
- **Save History**: Record and display previous step entries
- **Clean Interface**: Simple, centered layout with background image
- **Instant Updates**: No page reload required - live DOM updates
- **Reset Functionality**: Automatically resets counter to 0 after saving

## 🎯 How It Works

1. **INCREMENT**: Click the black button to add +1 to your step count
2. **SAVE**: Click the gray button to save your current count to history
3. **View History**: All saved entries appear below with " - " separator
4. **Auto-Reset**: Counter resets to 0 after each save

## 🛠️ Technologies Used

- **Vanilla JavaScript**: No frameworks - pure JS for DOM manipulation
- **HTML5**: Semantic markup with inline event handlers
- **CSS3**: Background images, custom fonts, and centered layout
- **Vite**: Lightning-fast development server with HMR
- **Trebuchet MS Font**: Clean, bold typography

## 📁 Project Structure

```
Scrim-s03i8nc/
├── index.html              # Main HTML with onclick handlers
├── index.js                # Counter logic and DOM manipulation
├── index.css               # Styling with background image
├── step1.jpg               # Background image asset
├── image.png               # App preview screenshot
├── package.json            # Vite dependencies and scripts
├── vite.config.js          # Vite configuration
└── README.md               # Project documentation
```

## 💻 Code Highlights

### JavaScript Functions

```javascript
function increment() {
  count += 1;
  countEl.textContent = count;
}

function save() {
  let countStr = count + " - ";
  saveEl.textContent += countStr;
  countEl.textContent = 0;
  count = 0;
}
```

### DOM Manipulation

- Uses `document.getElementById()` for element selection
- Updates UI with `textContent` (not `innerHTML`) for safety
- Inline `onclick` handlers for event handling

### Styling Approach

- Background image with `background-size: cover`
- Centered layout using `text-align: center` and margin-based positioning
- Simple color scheme: black increment button, gray save button

## 🚀 Getting Started

### Prerequisites

- Node.js (version 14 or higher)
- npm package manager

### Installation

1. **Clone or download the repository**

   ```bash
   git clone <your-repo-url>
   cd Scrim-s03i8nc
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Start development server**

   ```bash
   npm start
   # or
   npm run dev
   ```

4. **Open in browser**

   Vite will automatically open your default browser, or navigate to `http://localhost:5173`

### Build for Production

```bash
npm run build
```

### Preview Production Build

```bash
npm run preview
```

## 🎓 Learning Goals

This project demonstrates key JavaScript fundamentals:

- **DOM Manipulation**: Selecting and updating HTML elements
- **Event Handling**: Using onclick handlers to trigger functions
- **State Management**: Tracking counter value in a variable
- **String Concatenation**: Building history strings with saved values
- **Function Design**: Creating reusable `increment()` and `save()` functions

## 🔧 Development

This project uses Vite for fast development:

- **Hot Module Replacement**: Instant updates during development
- **Fast Build**: Optimized production builds
- **No Configuration**: Works out of the box with minimal setup

## 📚 Project Credits

This project was created as part of the **Frontend Developer Path** on [Scrimba.com](https://scrimba.com/). It demonstrates fundamental JavaScript concepts including DOM manipulation, event handling, and state management.

**Platform**: [Scrimba.com](https://scrimba.com/) - Interactive coding tutorials
**Course Link**: [Scrimba Frontend Path](https://scrimba.com/frontend-path-c0j)

## 📞 Contact

- **Developer**: Ali Hassan
- **Email**: [m.alihassan002@gmail.com](mailto:m.alihassan002@gmail.com)
- **LinkedIn**: [Ali Hassan](https://www.linkedin.com/in/ali-hassan-9ba69220b/)
- **Location**: Lahore, Pakistan
- **Role**: Full Stack Developer

---

_Built with ❤️ as part of learning vanilla JavaScript fundamentals_
