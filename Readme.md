# Doctify - Healthcare Telemedicine App

![Doctify Logo](https://via.placeholder.com/150x150.png?text=Doctify)

Doctify is a comprehensive healthtech platform designed to revolutionize access to healthcare by offering virtual consultations, physician discovery, and AI-powered health insights.

## 📱 Features

### Core Features
- **🔍 Find a Doctor** - Filter by specialty, location, language, and availability
- **💬 Virtual Consultations** - Secure video/voice/chat with licensed physicians
- **📊 Health Dashboard** - Personalized wellness recommendations
- **📝 E-Prescriptions & Medical Records** - Stored securely and shared easily

### Additional Features
- **Physician Directory** - Searchable by specialization, rating, insurance, gender, language
- **Health Insights & Recommendations** - AI-powered daily health tips
- **Centralized Medical Records** - Secure cloud storage for health documents
- **Cross-Platform Support** - iOS, Android, and Web

## 🛠️ Tech Stack

### Frontend
- **React Native** - Mobile app for iOS and Android
- **React Navigation** - For seamless app navigation
- **Axios** - API communication
- **AsyncStorage** - Local data persistence

### Backend
- **Node.js & Express** - Server-side API
- **MongoDB** - Database
- **Mongoose** - ODM for MongoDB
- **JWT** - Authentication
- **bcrypt** - Password hashing

## 🚀 Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- MongoDB (local or Atlas)
- React Native development environment

### Setting Up the Backend

1. Clone the repository
   ```bash
   git clone https://github.com/yourusername/doctify.git
   cd doctify
   ```

2. Install server dependencies
   ```bash
   cd server
   npm install
   ```

3. Create a `.env` file in the server directory with the following variables:
   ```
   PORT=5000
   MONGODB_URI=mongodb://localhost:27017/doctify
   JWT_SECRET=your_jwt_secret_key_here
   JWT_EXPIRES_IN=7d
   NODE_ENV=development
   ```

4. Start the server
   ```bash
   npm run dev
   ```

### Setting Up the Mobile App

1. Install client dependencies
   ```bash
   cd ../client
   npm install
   ```

2. Create a `config/constants.js` file with the API URL:
   ```javascript
   export const API_URL = 'http://localhost:5000/api';
   ```

3. Start the app
   ```bash
   # For iOS
   npx react-native run-ios
   
   # For Android
   npx react-native run-android
   ```

## 📂 Project Structure

```
doctify/
├── client/                  # Mobile app (React Native)
│   ├── App.js               # Entry point
│   ├── assets/              # Images, fonts, etc.
│   ├── components/          # Reusable UI components
│   ├── screens/             # App screens
│   ├── navigation/          # Navigation configuration
│   ├── services/            # API calls, authentication
│   └── utils/               # Helper functions
│
├── server/                  # Backend (Node.js)
│   ├── server.js            # Entry point
│   ├── config/              # Environment variables
│   ├── controllers/         # Request handlers
│   ├── models/              # Database models
│   ├── routes/              # API routes
│   ├── middleware/          # Custom middleware
│   └── utils/               # Helper functions
│
└── README.md                # Project documentation
```

## 🧪 API Endpoints

### Authentication
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login a user

### Doctors
- `GET /api/doctors` - Get all doctors
- `GET /api/doctors/:id` - Get a specific doctor
- `GET /api/doctors/specialties` - Get all specialties

### Appointments
- `POST /api/appointments` - Create a new appointment
- `GET /api/appointments/user` - Get user appointments
- `PUT /api/appointments/:id` - Update an appointment status

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📞 Contact

If you have any questions or feedback, please reach out to email

---

Made by Ojasva
