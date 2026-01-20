# Mental Wellness App 🧠💚

A comprehensive mental health and wellness web application built with the MERN stack that provides users with tools for mood tracking, meditation, journaling, and mental health assessment.

## 🌟 Features

- **Mood Tracker**: Track your daily moods and visualize your emotional patterns with interactive charts
- **Meditation & Mindfulness**: Access guided meditation sessions with audio playback
- **Mental Health Exercises**: Practice various therapeutic exercises and coping strategies
- **Journal**: Maintain a personal digital journal to track your thoughts and feelings
- **PHQ-9 Assessment**: Take standardized mental health assessments
- **Community Stories**: Read and share inspiring mental wellness stories
- **User Authentication**: Secure login and registration system
- **Testimonials**: Read user experiences and success stories

## 🛠️ Tech Stack

### Frontend (Client)
- **React 18.3.1** - UI library for building user interfaces
- **Vite 6.0.5** - Fast build tool and dev server
- **React Router DOM 7.1.1** - Client-side routing
- **Redux Toolkit 2.5.0** - State management
- **React Redux 9.2.0** - React bindings for Redux
- **Axios 1.7.9** - HTTP client for API requests
- **Tailwind CSS 3.4.17** - Utility-first CSS framework
- **DaisyUI 4.12.23** - Tailwind CSS component library
- **Chart.js 4.4.7** - Interactive charts
- **React Chart.js 2 5.3.0** - React wrapper for Chart.js
- **Framer Motion 11.18.0** - Animation library
- **React Icons 5.4.0** - Icon library
- **React H5 Audio Player** - Audio player component for meditation
- **React Toastify 11.0.2** - Toast notifications
- **React Wrap Balancer** - Better text wrapping

### Backend (Server)
- **Node.js** - JavaScript runtime
- **Express.js 4.21.2** - Web application framework
- **MongoDB** - NoSQL database
- **Mongoose 8.9.4** - MongoDB object modeling
- **JWT (jsonwebtoken 9.0.2)** - Authentication and authorization
- **Bcrypt 5.1.1** - Password hashing
- **CORS 2.8.5** - Cross-Origin Resource Sharing
- **Dotenv 16.4.7** - Environment variable management
- **Moment.js 2.30.1** - Date and time manipulation
- **Express Async Handler 1.2.0** - Async error handling

### Development Tools
- **ESLint** - Code linting
- **PostCSS** - CSS processing
- **Autoprefixer** - CSS vendor prefixing

## 📁 Project Structure

```
mental-wellness-app/
├── client/                      # Frontend application
│   ├── src/
│   │   ├── components/         # Reusable components
│   │   │   ├── Home.jsx
│   │   │   ├── Navbar.jsx
│   │   │   ├── Footer.jsx
│   │   │   ├── PieChart.jsx
│   │   │   └── ScrollTop.jsx
│   │   ├── pages/              # Page components
│   │   │   ├── Login.jsx
│   │   │   ├── Register.jsx
│   │   │   ├── MoodTracker.jsx
│   │   │   ├── Journal.jsx
│   │   │   ├── Mediation.jsx
│   │   │   ├── Exercises.jsx
│   │   │   ├── Features.jsx
│   │   │   ├── Stories.jsx
│   │   │   ├── Community.jsx
│   │   │   └── Testimonials.jsx
│   │   ├── features/           # Redux slices
│   │   │   ├── authSlice.js
│   │   │   └── authService.js
│   │   ├── app/                # Redux store
│   │   │   └── store.js
│   │   ├── utils/              # Utility functions and data
│   │   │   ├── benefitsData.js
│   │   │   ├── featureData.js
│   │   │   ├── mediationData.js
│   │   │   ├── storiesData.js
│   │   │   └── testimonialsData.js
│   │   ├── App.jsx             # Main app component
│   │   ├── main.jsx            # Entry point
│   │   └── apiService.js       # API configuration
│   ├── public/                 # Static assets
│   ├── index.html              # HTML template
│   ├── package.json            # Dependencies
│   ├── vite.config.js          # Vite configuration
│   ├── tailwind.config.js      # Tailwind CSS configuration
│   └── vercel.json             # Vercel deployment config
│
└── server/                      # Backend application
    ├── config/
    │   └── db.js               # Database configuration
    ├── models/
    │   ├── userModel.js        # User schema
    │   └── ResponseModel.js    # PHQ-9 response schema
    ├── routes/
    │   ├── userRoute.js        # User authentication routes
    │   └── phq9Routes.js       # PHQ-9 assessment routes
    ├── index.js                # Server entry point
    ├── package.json            # Dependencies
    └── vercel.json             # Vercel deployment config
```

## 🚀 Getting Started

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or cloud instance)
- npm or yarn

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd mental-wellness-app-main
   ```

2. **Install server dependencies**
   ```bash
   cd server
   npm install
   ```

3. **Install client dependencies**
   ```bash
   cd ../client
   npm install
   ```

4. **Set up environment variables**
   
   Create a `.env` file in the `server` directory:
   ```env
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret_key
   PORT=5000
   ```

5. **Run the application**

   **Start the server (in server directory):**
   ```bash
   npm start
   # or for development with auto-reload
   npm run server
   ```

   **Start the client (in client directory):**
   ```bash
   npm run dev
   ```

6. **Access the application**
   - Frontend: `http://localhost:5173` (Vite default port)
   - Backend API: `http://localhost:5000`

## 📝 Available Scripts

### Client
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

### Server
- `npm start` - Start server
- `npm run server` - Start server with auto-reload (watch mode)

## 🔐 Authentication

The app uses JWT (JSON Web Tokens) for authentication:
- User passwords are hashed using bcrypt before storage
- Protected routes require valid JWT tokens
- Tokens are stored in Redux state and used for API requests

## 📊 Key Features Details

### Mood Tracker
- Visual representation of mood patterns using Chart.js
- Track daily emotional states
- View historical mood data

### Meditation
- Audio player for guided meditation sessions
- Multiple meditation tracks
- User-friendly playback controls

### PHQ-9 Assessment
- Standardized mental health screening tool
- Store and track assessment results
- Monitor mental health progress over time

### Journal
- Private space for personal reflections
- Secure storage of journal entries
- Date-based organization

## 🌐 Deployment

The application is configured for deployment on Vercel:
- Both client and server have `vercel.json` configuration files
- Frontend: Static site deployment
- Backend: Serverless functions

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Author

Suraj

## 🙏 Acknowledgments

- Mental health resources and guidelines
- Open source community
- All contributors and testers

---

**Note:** This is a mental wellness application. If you're experiencing a mental health crisis, please contact a mental health professional or emergency services immediately.
