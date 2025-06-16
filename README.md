# ZoeFlockAdmin

**ZoeFlockAdmin** is a modern, full-stack Church Management System built with **Laravel 11** (Backend API) and **ReactJS** (Frontend UI). The system is designed to help churches manage members, attendance, events, donations, communication, and more.

*"The life and care of the flock, simplified."*

---

## ✨ Tech Stack

- **Backend:** Laravel 11 (PHP 8.2+)
- **Frontend:** React JS (with Vite bundler)
- **UI Framework:** Bootstrap 5
- **Database:** PostgreSQL
- **Authentication:** Laravel Breeze (Sanctum + React)
- **HTTP Client:** Axios
- **Queue System:** Laravel Queues (Redis or Database based)

---

## 🚀 Features

- ✅ **Member Management** - Complete CRUD operations for church members
- ✅ **Attendance Tracking** - Monitor service and event attendance
- ✅ **Groups & Ministries** - Organize members into groups and ministries
- ✅ **Event Scheduling** - Plan and manage church events
- ✅ **Donations & Finance** - Track donations and financial contributions
- ✅ **Staff & Volunteers** - Manage church staff and volunteer assignments
- ✅ **Secure Authentication** - Role-based access control
- ✅ **RESTful API** - Full API powered by Laravel Sanctum
- ✅ **Responsive Dashboard** - Modern admin interface with React + Bootstrap 5

---

## 📋 Requirements

- PHP 8.2 or higher
- Composer
- Node.js 16+ and npm/yarn
- PostgreSQL 12+
- Redis (optional, for queues)

---

## ⚙️ Installation

### 1️⃣ Clone Repository
```bash
git clone https://github.com/douglasderrick/zoeflockadmin.git
cd zoeflockadmin
```

### 2️⃣ Install Backend Dependencies
```bash
composer install
```

### 3️⃣ Setup Environment
```bash
cp .env.example .env
php artisan key:generate
```

Configure your database connection in `.env`:
```env
DB_CONNECTION=pgsql
DB_HOST=127.0.0.1
DB_PORT=5432
DB_DATABASE=zoeflockadmin
DB_USERNAME=your_username
DB_PASSWORD=your_password
```

### 4️⃣ Install Laravel Breeze (React + Sanctum)
```bash
composer require laravel/breeze --dev
php artisan breeze:install react
```

### 5️⃣ Install Frontend Dependencies
```bash
npm install
```

### 6️⃣ Run Database Migrations
```bash
php artisan migrate
```

### 7️⃣ Seed Database (Optional)
```bash
php artisan db:seed
```

### 8️⃣ Start Development Servers
```bash
# Terminal 1 - Laravel Backend
php artisan serve

# Terminal 2 - React Frontend
npm run dev
```

The application will be available at:
- Frontend: `http://localhost:5173`
- Backend API: `http://localhost:8000`

---

## 🔐 API Authentication

ZoeFlockAdmin uses **Laravel Sanctum** for API authentication. The system provides:

- Token-based authentication for SPA (Single Page Application)
- CSRF protection
- API token management
- Role-based permissions

Once a user registers or logs in, frontend requests automatically include authentication tokens via Axios interceptors.

---

## 📁 Project Structure

```
zoeflockadmin/
├── app/                    # Laravel backend logic
│   ├── Http/Controllers/   # API controllers
│   ├── Models/            # Eloquent models
│   └── Services/          # Business logic services
├── database/
│   ├── migrations/        # Database schema
│   └── seeders/          # Sample data
├── resources/
│   └── js/               # React frontend application
│       ├── Components/   # Reusable React components
│       ├── Pages/        # Page components
│       └── Layouts/      # Layout components
├── routes/
│   ├── api.php          # API routes
│   └── web.php          # Web routes
└── public/              # Public assets
```

---

*For complete API documentation, visit `/api/documentation` after installation.*

---

## 🛠️ Development

### Running Tests
```bash
# Backend tests
php artisan test

# JavaScript/React formatting (Prettier)
npm run format
```

### Building for Production
```bash
npm run build
php artisan optimize
```

---

## 🎯 Roadmap

### Version 1.0 (Current)
- ✅ Member management system
- ✅ Church groups and ministries
- ✅ Event scheduling
- ✅ Attendance tracking
- ✅ Staff and volunteer management
- ✅ Admin dashboard interface
- ✅ Email notifications
- ✅ API documentation

### Version 1.1 (Planned)
- 📱 Mobile app (React Native)
- 📊 Advanced reporting and analytics
- 💬 Internal messaging system
- 📧 Bulk email campaigns
- 🔗 Third-party integrations (PayPal, Stripe)

### Version 2.0 (Future)
- 📱 Mobile-first responsive design
- 🌐 Multi-language support
- ☁️ Cloud deployment options
- 🔄 Real-time notifications
- 📈 Advanced dashboard analytics

---
## 🙏 Support Development
Buy Me a Coffee ☕️ to support development: [Buy Me a Coffee](https://www.buymeacoffee.com/douglasderrick)
## 

## 🤝 Contributing
We welcome contributions to ZoeFlockAdmin! To contribute:
1. Fork the repository
2. Create a new branch (`git checkout -b feature/YourFeature`)
3. Make your changes and commit them (`git commit -m 'Add new feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request with a clear description of your changes
6. Ensure your code adheres to the project's coding standards
7. Write tests for new features or bug fixes
8. Update documentation if necessary
9. Follow the project's commit message guidelines
10. Be respectful and constructive in code reviews
11. Keep your pull request focused on a single feature or fix
12. Respond to feedback and make necessary changes

---

## 🐛 Issues & Support

If you encounter any issues or need support:

1. Check the [Issues](https://github.com/douglasderrick/zoeflockadmin/issues) page
2. Search existing issues before creating a new one
3. Provide detailed information about the problem
4. Include steps to reproduce the issue

---

## 📄 License

ZoeFlockAdmin is open-sourced software licensed under the [MIT License](LICENSE).

---

## 🙏 Acknowledgments

- Laravel team for the amazing framework
- React team for the powerful UI library
- Bootstrap team for the responsive CSS framework
- All contributors who help make this project better

---

## 📞 Contact

- **Project Link:** [https://github.com/douglasderrick/zoeflockadmin](https://github.com/douglasderrick/zoeflockadmin)
- **Documentation:** [Coming Soon]
- **Demo:** [Coming Soon]

---

*Built with ❤️ for churches worldwide*