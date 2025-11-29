# Clinic-reservation-system
graduation project
# 🏥 Clinic Reservation System

A comprehensive web-based clinic reservation system that allows patients to book appointments, manage their medical records, and enables healthcare providers to manage their schedules efficiently.

## ✨ Features

### For Patients
- 📅 **Easy Appointment Booking** - Schedule appointments with preferred doctors
- 👤 **Patient Profile Management** - Update personal and medical information
- 📋 **Appointment History** - View past and upcoming appointments
- 🔔 **Notifications** - Receive appointment reminders and updates
- 💊 **Medical Records Access** - View prescriptions and test results

### For Doctors
- 🗓️ **Schedule Management** - Set availability and manage appointments
- 👥 **Patient Management** - Access patient records and history
- 📝 **Prescription Management** - Create and manage prescriptions
- 📊 **Dashboard** - Overview of daily appointments and statistics

### For Admins
- 🏢 **Clinic Management** - Manage doctors, patients, and appointments
- 📈 **Analytics & Reports** - Generate reports and view system statistics
- ⚙️ **System Configuration** - Configure system settings and parameters

## 🚀 Tech Stack

### Frontend
- React.js
- HTML5/CSS3
- JavaScript (ES6+)
- Bootstrap/Material-UI

### Backend
- Node.js
- Express.js
- MongoDB
- JWT Authentication

## 📋 Prerequisites

Before you begin, ensure you have the following installed:
- Node.js (v14 or higher)
- npm or yarn
- MongoDB (v4.4 or higher)
- Git

## 🛠️ Installation

### 1. Clone the Repository
```bash
git clone https://github.com/omarwael36/Clinic-reservation-system.git
cd Clinic-reservation-system
```

### 2. Install Backend Dependencies
```bash
cd backend
npm install
```

### 3. Install Frontend Dependencies
```bash
cd ../frontend
npm install
```

### 4. Environment Configuration

#### Backend (.env)
Create a `.env` file in the `backend` directory:
```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/clinic-reservation
JWT_SECRET=your_jwt_secret_key_here
JWT_EXPIRE=7d
NODE_ENV=development
```

#### Frontend (.env)
Create a `.env` file in the `frontend` directory:
```env
REACT_APP_API_URL=http://localhost:5000/api
```

## 🚀 Running the Application

### Development Mode

#### Start Backend Server
```bash
cd backend
npm start
# or for development with hot reload
npm run dev
```
The backend server will run on `http://localhost:5000`

#### Start Frontend Development Server
```bash
cd frontend
npm start
```
The frontend will run on `http://localhost:3000`

### Production Build

#### Build Frontend
```bash
cd frontend
npm run build
```

#### Start Production Server
```bash
cd backend
npm run production
```

## 🐳 Docker Deployment

### Using Docker Compose
```bash
docker-compose up -d
```

### Build Individual Containers

#### Frontend
```bash
cd frontend
docker build -t clinic-frontend .
docker run -p 3000:3000 clinic-frontend
```

#### Backend
```bash
cd backend
docker build -t clinic-backend .
docker run -p 5000:5000 clinic-backend
```

## 📁 Project Structure

```
Clinic-reservation-system/
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── utils/
│   │   └── App.js
│   ├── Dockerfile
│   └── package.json
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── config/
│   ├── utils/
│   ├── server.js
│   └── package.json
├── docker-compose.yml
└── README.md
```

## 🔑 Default Login Credentials

### Admin
- Email: `admin@clinic.com`
- Password: `admin123`

### Doctor
- Email: `doctor@clinic.com`
- Password: `doctor123`

### Patient
- Email: `patient@clinic.com`
- Password: `patient123`

> **Note:** Change these credentials immediately after first login in production.

## 🧪 Running Tests

### Backend Tests
```bash
cd backend
npm test
```

### Frontend Tests
```bash
cd frontend
npm test
```

## 📚 API Documentation

API documentation is available at `http://localhost:5000/api-docs` when running in development mode.

### Main Endpoints

#### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout

#### Appointments
- `GET /api/appointments` - Get all appointments
- `POST /api/appointments` - Create new appointment
- `PUT /api/appointments/:id` - Update appointment
- `DELETE /api/appointments/:id` - Cancel appointment

#### Patients
- `GET /api/patients` - Get all patients
- `GET /api/patients/:id` - Get patient details
- `PUT /api/patients/:id` - Update patient info

#### Doctors
- `GET /api/doctors` - Get all doctors
- `GET /api/doctors/:id` - Get doctor details
- `GET /api/doctors/:id/schedule` - Get doctor schedule

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


## 🙏 Acknowledgments

- Thanks to all contributors who have helped with this project
- Inspired by modern healthcare management systems
- Built with love for the healthcare community

## 📞 Support

For support, email omar@example.com or open an issue in the GitHub repository.

## 🔮 Future Enhancements

- [ ] SMS/Email notifications
- [ ] Video consultation integration
- [ ] Payment gateway integration
- [ ] Multi-language support
- [ ] Mobile application (React Native)
- [ ] AI-powered appointment recommendations
- [ ] Integration with electronic health records (EHR)

## 📊 Screenshots

![WhatsApp Image 2025-11-29 at 5 09 57 PM](https://github.com/user-attachments/assets/011986ea-24d3-441e-a4a8-31bd974099e7)
![WhatsApp Image 2025-11-29 at 5 09 55 PM](https://github.com/user-attachments/assets/7bf62896-0377-460a-91d2-dc7de901cc02)




⭐ If you find this project useful, please consider giving it a star on GitHub!

