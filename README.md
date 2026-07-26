# BunnyEra Pay

**Enterprise Payment Infrastructure Platform**

Multi-currency wallet, virtual card, payment gateway, merchant API, and financial management system.

## 📋 Product Overview

BunnyEra Pay is a comprehensive payment infrastructure platform designed for enterprises. It provides a complete suite of financial services including multi-currency wallet management, virtual card issuance, payment gateway integration, and merchant API access.

## ✨ Core Features

- **Multi-Currency Wallet**: Manage funds in multiple currencies with real-time conversion
- **Virtual Card Issuance**: Create and manage virtual cards for payments and transactions
- **Payment Gateway**: Accept payments from various channels and methods
- **Merchant API**: Integrate payments into third-party applications
- **Transaction Ledger**: Complete audit trail and transaction history
- **Risk Management**: Fraud detection and risk assessment
- **Webhook System**: Real-time event notifications
- **Financial Settlement**: Automated settlement and reconciliation
- **Admin Dashboard**: Comprehensive merchant and transaction management

## 🏗️ Architecture

The platform is built as a modular monorepo with clear separation of concerns:

```
Backend (Java/Spring Boot)
├── Authentication & Authorization
├── User Management
├── Wallet Services
├── Transaction Ledger
├── Payment Processing
├── Merchant Management
├── Virtual Card Management
├── Webhook Services
└── Risk Management

Frontend (Admin Dashboard)
└── Management Portal

Mobile (Flutter)
└── User App

Database (PostgreSQL)
└── Schema & Migrations

Documentation
└── API, Architecture, Database
```

## 🛠️ Technology Stack

### Backend
- **Runtime**: Java 21
- **Framework**: Spring Boot 3
- **Security**: Spring Security
- **Database**: PostgreSQL
- **Cache**: Redis
- **Message Queue**: RabbitMQ
- **Container**: Docker

### Frontend
- React/Vue.js (to be determined)
- Tailwind CSS
- TypeScript

### Mobile
- Flutter (for cross-platform support)

### DevOps
- Docker & Docker Compose
- Nginx (Reverse Proxy)

## 📁 Repository Structure

```
bunnyera-pay/
├── backend/                    # Java Spring Boot backend
│   ├── src/
│   │   ├── auth/              # Authentication & Authorization
│   │   ├── user/              # User Management
│   │   ├── wallet/            # Wallet Services
│   │   ├── ledger/            # Transaction Ledger
│   │   ├── payment/           # Payment Processing
│   │   ├── merchant/          # Merchant Management
│   │   ├── card/              # Virtual Card Management
│   │   ├── webhook/           # Webhook Services
│   │   └── risk/              # Risk Management
│   ├── pom.xml
│   └── Dockerfile
│
├── frontend/                   # Admin Dashboard & Merchant Portal
│   ├── admin/                 # Admin Dashboard
│   └── merchant/              # Merchant Portal
│
├── mobile/                     # Flutter Mobile App
│   └── flutter-app/
│
├── database/                   # Database Schemas & Migrations
│   ├── schema.sql
│   └── migrations/
│
├── docs/                       # Documentation
│   ├── API.md
│   ├── DATABASE.md
│   └── ARCHITECTURE.md
│
├── deploy/                     # Deployment Configuration
│   ├── docker-compose.yml
│   └── nginx/
│
├── .gitignore
├── README.md
└── LICENSE
```

## 🚀 Installation

### Prerequisites
- Docker & Docker Compose
- Java 21 (for local development)
- PostgreSQL 15+
- Redis 7+
- Node.js 18+ (for frontend)
- Flutter SDK (for mobile)

### Quick Start with Docker

```bash
# Clone the repository
git clone https://github.com/bunnyera-org/bunnyera-pay.git
cd bunnyera-pay

# Start services with Docker Compose
docker-compose up -d

# Services will be available at:
# API: http://localhost:8080
# Admin Dashboard: http://localhost:3000
# Database: localhost:5432
# Redis: localhost:6379
```

### Local Development

See [Development Guide](docs/DEVELOPMENT.md) for detailed setup instructions.

## 👨‍💻 Development

### Backend
```bash
cd backend
./mvnw spring-boot:run
```

### Frontend
```bash
cd frontend/admin
npm install
npm start
```

### Mobile
```bash
cd mobile/flutter-app
flutter pub get
flutter run
```

## 📚 API Documentation

Full API documentation is available at [docs/API.md](docs/API.md)

### Key Endpoints
- Authentication: `/api/v1/auth/*`
- User Management: `/api/v1/users/*`
- Wallet: `/api/v1/wallets/*`
- Transactions: `/api/v1/transactions/*`
- Cards: `/api/v1/cards/*`
- Merchants: `/api/v1/merchants/*`

## 🗺️ Roadmap

### Phase 1 (Q3 2026)
- [ ] Core wallet functionality
- [ ] Basic payment processing
- [ ] Admin dashboard
- [ ] User authentication

### Phase 2 (Q4 2026)
- [ ] Virtual card issuance
- [ ] Merchant API
- [ ] Risk management
- [ ] Mobile app MVP

### Phase 3 (Q1 2027)
- [ ] Multi-currency support
- [ ] Advanced analytics
- [ ] Settlement automation
- [ ] Third-party integrations

### Phase 4 (Q2 2027)
- [ ] Compliance & Reporting
- [ ] High-volume optimization
- [ ] Enterprise features

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Support

For questions, issues, or contributions, please open an issue on GitHub or contact the development team.

---

**Made with ❤️ by BunnyEra Team**
