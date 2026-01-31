# 📚 UniSwap

> **UniSwap is a responsive web platform that enables university students to list, discover, and exchange books and study resources locally, promoting sustainability, affordability, and community sharing.**

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Platform](https://img.shields.io/badge/platform-web-brightgreen.svg)
![Status](https://img.shields.io/badge/status-in%20development-yellow.svg)

---

## 🎯 Overview

UniSwap addresses the challenge of expensive textbooks and sustainability concerns in higher education by creating a peer-to-peer marketplace for students to share books, notes, and study equipment. Built with mobile-first design principles and WCAG 2.1 AA accessibility compliance.

---

## 🏗️ System Architecture

<p align="center">
  <img src="docs/diagrams/UniSwap_Architecture.svg" alt="System Architecture" width="100%">
</p>

---

## ✨ Features Overview

<p align="center">
  <img src="docs/diagrams/UniSwap_Features.svg" alt="Features Overview" width="100%">
</p>

### 📋 Listings (Core)
- Create listings with photos, titles, and descriptions
- Specify item condition
- Categorise by: **Subject**, **Module code**, **Type** (Book / Notes / Equipment)

### 👤 User Management (Core)
- Student registration & login (university email only)
- User profiles with display name, course info, and contact preferences
- GDPR compliant with minimal personal data collection

### 🔍 Search & Discovery
- Keyword search across all listings
- Filters: Category, Subject, Availability, Location zones

### 🔗 External Integrations
- **Open Library API**: Auto-populate book details using ISBN
- **Cloudinary**: Image storage and optimization
- **Maps API**: Display pickup zones (optional)

### 💬 Communication
- In-app request system with Accept/Decline functionality

### ⭐ Community & Gamification
- 1-5 star rating system
- Points: +10 per shared item
- Badges: 🥇 First Share, 🌱 Sustainability Supporter

### 📊 Analytics Dashboard
- Personal impact: Items shared, money saved
- Community impact: Total reused items, CO₂ reduction

---

## 🗺️ User Journey

<p align="center">
  <img src="docs/diagrams/UniSwap_UserFlow.svg" alt="User Flow" width="100%">
</p>

---

## � Technology Stack

<p align="center">
  <img src="docs/diagrams/UniSwap_TechStack.svg" alt="Tech Stack" width="100%">
</p>

| Layer | Technologies |
|-------|-------------|
| **Frontend** | HTML5, CSS3, JavaScript, React/Next.js |
| **Backend** | Node.js, Express.js, RESTful API |
| **Database** | PostgreSQL |
| **Cloud** | Cloudinary (Images), Open Library API |
| **Deployment** | Netlify/Vercel (Frontend), Render/Railway (Backend) |
| **Security** | HTTPS, JWT, GDPR Compliant, WCAG 2.1 AA |

---

## ⚙️ Non-Functional Requirements

| Requirement | Implementation |
|-------------|----------------|
| **Responsive Design** | Mobile-first approach, desktop & mobile layouts |
| **Accessibility** | WCAG 2.1 AA (alt text, keyboard nav, high contrast) |
| **UX & Navigation** | Simple navigation (Browse, Add Item, Profile) |
| **Security & Privacy** | Hashed passwords, HTTPS, data minimisation |
| **Testing & CI** | Unit tests, GitHub Actions CI |

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v18+)
- PostgreSQL
- npm or yarn

### Installation

```bash
# Clone the repository
git clone https://github.com/DipKumar0001/UniSwap.git
cd UniSwap

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env

# Run database migrations
npm run migrate

# Start development server
npm run dev
```

### Environment Variables

```env
DATABASE_URL=postgresql://user:password@localhost:5432/uniswap
CLOUDINARY_URL=cloudinary://api_key:api_secret@cloud_name
OPEN_LIBRARY_API=https://openlibrary.org/api
SESSION_SECRET=your-secret-key
```

---

## 📁 Project Structure

```
UniSwap/
├── docs/
│   └── diagrams/        # Architecture & flow diagrams (SVG)
├── public/              # Static assets
├── src/
│   ├── components/      # UI components
│   ├── pages/           # Page components
│   ├── services/        # API services
│   └── styles/          # CSS/SCSS files
├── server/
│   ├── controllers/     # Route controllers
│   ├── models/          # Database models
│   └── routes/          # API routes
├── tests/               # Test files
└── .github/workflows/   # CI/CD pipelines
```

---

## 🧪 Testing

```bash
npm test              # Run unit tests
npm run test:coverage # Run with coverage
npm run lint          # Run linting
```

---

## 🗺️ Roadmap

- [x] Project setup & architecture diagrams
- [ ] User authentication system
- [ ] Listings CRUD functionality
- [ ] Search & filter implementation
- [ ] Open Library API integration
- [ ] Request/response system
- [ ] Rating & gamification features
- [ ] Analytics dashboard
- [ ] Production deployment

---

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 👥 Team

- **Dipesh Kumar Yadav** - [GitHub](https://github.com/DipKumar0001)
- **Ankesh Kumar Baitha** - [GitHub](https://github.com/ankeshrajak)
- **Sohan Giri** - [GitHub](https://github.com/sohan0911)
- **Rabin Kumar Dahal** - [GitHub](https://github.com/Raybin-coder)
- **ASHIKHA AMBALATHUVEETTIL ASHRAF** - [GitHub](https://github.com/Ashikha2005)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

<p align="center">
  <strong>🌱 Promoting sustainability, one textbook at a time.</strong>
</p>
