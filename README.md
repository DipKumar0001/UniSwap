# 📚 UniSwap

> **UniSwap is a responsive web platform that enables university students to list, discover, and exchange books and study resources locally, promoting sustainability, affordability, and community sharing.**

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Platform](https://img.shields.io/badge/platform-web-brightgreen.svg)
![Status](https://img.shields.io/badge/status-in%20development-yellow.svg)

---

## 🎯 Overview

UniSwap addresses the challenge of expensive textbooks and sustainability concerns in higher education by creating a peer-to-peer marketplace for students to share books, notes, and study equipment. Built with mobile-first design principles and WCAG 2.1 AA accessibility compliance.

---

## ✨ Features

### 📋 Listings (Core)
- Create listings with photos, titles, and descriptions
- Specify item condition
- Categorise by:
  - **Subject** area
  - **Module code**
  - **Type** (Book / Notes / Equipment)

### 👤 User Management (Core)
- Student registration & login (university email only)
- User profiles with:
  - Display name
  - Course information
  - Contact preferences
- GDPR compliant with minimal personal data collection
- Full user control over listings

### 🔍 Search & Discovery
- **Keyword search** across all listings
- **Filters**:
  - Category
  - Subject
  - Availability
  - Location (On-campus zones: Library / Main Campus)

### 🔗 External Integrations
- **Open Library API**: Auto-populate book details using ISBN
- **Book Cover Images**: Automatic fetching from Open Library
- **Maps API** (Optional): Display pickup zones

### 💬 Communication
- In-app request system:
  - "Request Item" functionality
  - Accept / Decline responses

### ⭐ Community Features
- Simple rating system (1–5 stars)

### 🎮 Gamification
- **Points System**: +10 points per shared item
- **Badges**:
  - 🥇 First Share
  - 🌱 Sustainability Supporter
- Ethical design with transparent scoring (no addictive loops)

### 📊 Analytics Dashboard
**Personal Impact:**
- Items shared count
- Estimated money saved

**Community Impact:**
- Total reused items
- Estimated CO₂ reduction

---

## ⚙️ Non-Functional Requirements

| Requirement | Implementation |
|-------------|----------------|
| **Responsive Design** | Mobile-first approach, desktop & mobile layouts |
| **Accessibility** | WCAG 2.1 AA compliant (alt text, keyboard nav, high contrast, screen-reader labels) |
| **UX & Navigation** | Simple navigation (Browse, Add Item, Profile), clear CTAs |
| **Security & Privacy** | Hashed passwords, HTTPS, data minimisation, GDPR compliance |
| **Testing & CI** | Unit tests (Login, Listings), GitHub Actions CI |

---

## 🏗️ Tech Stack

### Frontend
- HTML5 / CSS3 / JavaScript
- Responsive design framework
- Deployment: **Netlify** / **Vercel**

### Backend
- Node.js / Express (or similar)
- RESTful API architecture
- Deployment: **Render** / **Railway**

### Database
- **PostgreSQL**

### Media Storage
- **Cloudinary** for image hosting

### External APIs
- **Open Library API** – Book metadata & covers
- **Maps API** – Pickup zone display (optional)

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
# Edit .env with your configuration

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
├── public/              # Static assets
├── src/
│   ├── components/      # UI components
│   ├── pages/           # Page components
│   ├── services/        # API services
│   ├── utils/           # Utility functions
│   └── styles/          # CSS/SCSS files
├── server/
│   ├── controllers/     # Route controllers
│   ├── models/          # Database models
│   ├── routes/          # API routes
│   └── middleware/      # Custom middleware
├── tests/               # Test files
├── .github/
│   └── workflows/       # CI/CD pipelines
└── docs/                # Documentation
```

---

## 🧪 Testing

```bash
# Run unit tests
npm test

# Run tests with coverage
npm run test:coverage

# Run linting
npm run lint
```

---

## 📱 Screenshots

*Coming soon...*

---

## 🗺️ Roadmap

- [x] Project setup & architecture
- [ ] User authentication system
- [ ] Listings CRUD functionality
- [ ] Search & filter implementation
- [ ] Open Library API integration
- [ ] Request/response system
- [ ] Rating system
- [ ] Gamification features
- [ ] Analytics dashboard
- [ ] Production deployment

---

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 👥 Team

- **Dip Kumar** - [GitHub](https://github.com/DipKumar0001)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgements

- [Open Library](https://openlibrary.org/) for book metadata API
- [Cloudinary](https://cloudinary.com/) for image hosting
- All contributors and testers

---

<p align="center">
  <strong>🌱 Promoting sustainability, one textbook at a time.</strong>
</p>
