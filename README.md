# AI Chat 💬

A full-stack AI-powered chat application built with Google's Gemini API, featuring both web and mobile clients with a robust Node.js backend.

## 🌟 Features

- **Multi-platform Support**: Web application and mobile app (iOS/Android)
- **AI-Powered Conversations**: Integrated with Google Gemini API for intelligent responses
- **Real-time Chat**: Seamless messaging experience across platforms
- **Responsive Design**: Optimized for desktop and mobile devices
- **Cross-platform Compatibility**: Shared codebase for mobile platforms using React Native

## 🏗️ Architecture

```
ai-chat/
├── web-client/          # React web application
├── app-client/          # React Native Expo mobile app
├── server/              # Node.js backend server
└── README.md
```

## 🚀 Tech Stack

### Frontend
- **Web Client**: React.js
- **Mobile Client**: React Native with Expo
- **Styling**: CSS/Styled Components

### Backend
- **Server**: Node.js
- **API Integration**: Google Gemini API
- **Runtime**: Express.js (assumed)

### External Services
- **AI Provider**: Google Gemini API

## 📋 Prerequisites

Before running this application, make sure you have:

- [Node.js](https://nodejs.org/) (v16 or higher)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)
- [Expo CLI](https://docs.expo.dev/get-started/installation/) (for mobile development)
- Google Gemini API key

## 🛠️ Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com/abhishekgurjarin/ai-chat.git
cd ai-chat
```

### 2. Server Setup
```bash
cd server
npm install

# Create environment file
cp .env.example .env

# Add your Gemini API key to .env
GEMINI_API_KEY=your_gemini_api_key_here
PORT=3000
```

### 3. Web Client Setup
```bash
cd ../web-client
npm install
```

### 4. Mobile App Setup
```bash
cd ../app-client
npm install

# For iOS (macOS only)
npx pod-install ios
```

## 🚀 Running the Application

### Start the Server
```bash
cd server
npm start
# Server will run on http://localhost:3000
```

### Start the Web Client
```bash
cd web-client
npm start
# Web app will run on http://localhost:3001
```

### Start the Mobile App
```bash
cd app-client
npm start
# or
expo start

# Then use Expo Go app to scan QR code
# or run on simulator/emulator
npx expo run:ios     # for iOS
npx expo run:android # for Android
```

## 🌐 API Configuration

### Environment Variables

Create a `.env` file in the server directory:

```env
GEMINI_API_KEY=your_gemini_api_key_here
PORT=3000
NODE_ENV=development

# Optional: Database configuration
DB_HOST=localhost
DB_PORT=5432
DB_NAME=ai_chat
```

### Getting Gemini API Key

1. Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Create a new API key
3. Copy the key to your `.env` file

## 📱 Platform Support

### Web Client
- ✅ Chrome, Firefox, Safari, Edge
- ✅ Responsive design for mobile browsers
- ✅ Progressive Web App features

### Mobile App
- ✅ iOS (iPhone/iPad)
- ✅ Android
- ✅ Cross-platform native performance

## 🔧 Development

### Project Structure

```
web-client/
├── src/
│   ├── components/      # Reusable UI components
│   ├── pages/          # Page components
│   ├── services/       # API services
│   └── utils/          # Utility functions

app-client/
├── src/
│   ├── components/     # React Native components
│   ├── screens/        # Screen components
│   ├── services/       # API services
│   └── navigation/     # Navigation setup

server/
├── routes/             # API routes
├── controllers/        # Route handlers
├── middleware/         # Custom middleware
└── utils/              # Server utilities
```

### Available Scripts

#### Server
```bash
npm start          # Start production server
npm run dev        # Start development server with hot reload
npm test           # Run tests
```

#### Web Client
```bash
npm start          # Start development server
npm run build      # Build for production
npm test           # Run tests
```

#### Mobile App
```bash
npm start          # Start Expo development server
npm run build      # Build for production
npm test           # Run tests
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙋‍♂️ Author

**Abhishek Boadgurjar**
- GitHub: [@abhishekgurjarin](https://github.com/abhishekgurjarin)

## 🐛 Issues

If you encounter any issues or have suggestions, please [create an issue](https://github.com/abhishekgurjarin/ai-chat/issues).

## ⭐ Show your support

Give a ⭐️ if this project helped you!

---

Built with ❤️ using React, React Native, Node.js, and Google Gemini API
