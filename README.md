# Sigo.Cards - Digital Invitation Platform

A modern, professional, and mobile-friendly platform for creating, managing, and sending personalized digital invitations at scale.

## Features

### Core Features
- **Event Management** - Create and manage multiple events
- **Invitation Designer** - Upload custom designs or use professional templates
- **Bulk Card Generation** - Generate thousands of personalized invitation cards
- **Unique QR Codes & Links** - Each guest gets a unique QR code and invitation link
- **Multi-Channel Distribution** - Send via WhatsApp, SMS, Email
- **RSVP Management** - Track guest responses in real-time
- **Check-in System** - Scan QR codes for event check-in
- **Analytics & Reports** - Comprehensive event analytics and insights

### Guest Management
- Upload guest lists via Excel/CSV
- Bulk import with validation
- Search and filter guests
- Track RSVP status
- Send reminders
- Export guest data

### Platform Features
- **Modern Dashboard** - Intuitive event overview and analytics
- **Template Library** - Pre-designed professional templates
- **Bulk Export** - Download invitations as PDF, PNG, or ZIP
- **Admin Accounts** - Multi-user management with role-based access
- **Settings & Customization** - Branding, notifications, payment integration
- **Responsive Design** - Perfect on Android, Tablet, and Desktop

## Tech Stack

### Frontend
- React 18+ with TypeScript
- Tailwind CSS for styling
- Shadcn/ui component library
- Zustand for state management
- React Query for data fetching
- React Router for navigation
- Vite for bundling

### Backend
- Node.js with Express.js
- PostgreSQL for database
- JWT authentication
- Multer for file uploads
- QR Code generation library
- CSV parsing
- Twilio/Firebase for SMS/WhatsApp

### Mobile
- React Native / Expo for cross-platform
- Native camera access for QR code scanning

### DevOps
- Docker for containerization
- GitHub Actions for CI/CD
- AWS/Vercel for deployment

## Project Structure

```
sigo-cards/
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── hooks/
│   │   ├── store/
│   │   ├── utils/
│   │   └── App.tsx
│   └── package.json
├── backend/
│   ├── src/
│   │   ├── routes/
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── middleware/
│   │   ├── services/
│   │   └── server.ts
│   └── package.json
├── mobile/
│   ├── src/
│   └── package.json
└── docker-compose.yml
```

## Getting Started

### Prerequisites
- Node.js 18+
- PostgreSQL 14+
- Docker & Docker Compose

### Installation

1. Clone the repository
```bash
git clone https://github.com/johnsonsimba68-design/sigo-cards.git
cd sigo-cards
```

2. Install dependencies
```bash
# Frontend
cd frontend && npm install

# Backend
cd ../backend && npm install
```

3. Configure environment variables
```bash
# Backend .env
DATABASE_URL=postgresql://user:password@localhost:5432/sigo_cards
JWT_SECRET=your_secret_key
TWILIO_ACCOUNT_SID=your_twilio_sid
TWILIO_AUTH_TOKEN=your_twilio_token
```

4. Start development servers
```bash
# Terminal 1: Frontend
cd frontend && npm run dev

# Terminal 2: Backend
cd backend && npm run dev

# Terminal 3: Database
docker-compose up
```

## Usage

Visit `http://localhost:3000` to access the platform.

## License

MIT

## Support

For issues and feature requests, please use GitHub Issues.
