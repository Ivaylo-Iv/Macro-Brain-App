# 🧠 Macro Brain - Face Detection App

A sleek and interactive face detection application built with React and powered by the Clarifai AI API. Detect faces in any image with stunning visual effects and user authentication.

## ✨ Features

- **Face Detection**: Upload or paste image URLs to detect faces in real-time using the Clarifai API
- **User Authentication**: Sign up and sign in to track your detection history
- **Detection Counter**: Keep track of your total detections with an entry counter
- **Bounding Boxes**: Visual indicators around detected faces for precise localization
- **Smooth Animations**: Beautiful particle effects and parallax tilt interactions
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **Stylish UI**: Modern, gradient-based design with tachyons CSS framework

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- A Clarifai API key

### Installation

1. Clone the repository:

```bash
git clone https://github.com/ivayloivanov/macro-brain.git
cd macro-brain
```

2. Install dependencies:

```bash
npm install
```

3. Start the development server:

```bash
npm start
```

The app will open in your browser at `http://localhost:3000`

## 📚 Project Structure

```
src/
├── components/          # React components
│   ├── BG.js           # Background particle effects
│   ├── ImgDisplay.js   # Image display with detection boxes
│   ├── ImgLinkForm.js  # Image URL input form
│   ├── Navigation.js   # Navigation bar
│   ├── Rank.js         # User ranking/counter display
│   ├── SignIn.js       # Sign in component
│   └── SignUp.js       # Sign up component
├── containers/
│   └── App.js          # Main app container and logic
├── style/              # CSS stylesheets
└── fonts/              # Custom fonts
```

## 🛠 Technology Stack

- **React** - UI framework
- **Clarifai API** - Face detection AI service
- **Tachyons** - CSS utility framework
- **React Parallax Tilt** - 3D tilt effects
- **React TSParticles** - Particle animation effects

## 📦 Available Scripts

### `npm start`

Runs the app in development mode. Open [http://localhost:3000](http://localhost:3000) to view it in your browser. The page reloads when you make changes.

### `npm test`

Launches the test runner in interactive watch mode.

### `npm build`

Builds the app for production to the `build` folder. It correctly bundles React in production mode and optimizes the build for the best performance.

## 🌐 Backend Integration

This is the **frontend** repository. The backend API for user authentication and entry management is located in a separate repository.

The frontend communicates with the backend for:

- User registration and authentication
- Storing and retrieving user data (name, email, entry count)
- Maintaining user session information

Ensure your backend API is running and the endpoints are properly configured in the App component.

## 💡 How It Works

1. **User Authentication**: Sign up or sign in with your credentials
2. **Enter Image URL**: Paste a URL of an image containing faces
3. **Detect Faces**: Click the "Detect" button to analyze the image
4. **View Results**: The app displays the image with bounding boxes around detected faces
5. **Track Progress**: Your detection count increases with each successful detection

## 🎨 Customization

### Add Your Own Clarifai API Key

Open `src/containers/App.js` and update the API key:

```javascript
const app = new Clarifai.App({
  apiKey: "YOUR_API_KEY_HERE",
});
```

### Modify Styling

- Global styles: `src/style/global.css`
- Component-specific styles: Check corresponding CSS files in `src/style/`
- Responsive design: `src/style/responsive.css`

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👨‍💻 Author

Created by Ivaylo Ivanov

---

**Note**: Make sure the backend API is running separately for full functionality. Check the backend repository for setup instructions.
