# README - MVP-PRO Tech Company Home Page

![MVP-PRO Logo](./docs/logo.png)

## 🚀 Project Overview

**MVP-PRO** is a modern, minimally viable product for a tech company's home page. Built with cutting-edge technologies, featuring a beautiful responsive design and interactive UI.

### Tech Stack

- **Frontend**: Next.js 14, React 18, Tailwind CSS, TypeScript
- **Backend**: Node.js, Express.js, TypeScript
- **Infrastructure**: Nginx, Kong API Gateway, Docker, Docker Compose
- **Database**: Ready for integration (PostgreSQL, MongoDB)

## 📋 Features

✅ Modern interactive hero section
✅ Animated feature cards
✅ Service offerings showcase
✅ Responsive design (mobile-first)
✅ Dark mode support
✅ Professional footer
✅ RESTful API backend
✅ Docker containerization
✅ Nginx reverse proxy
✅ Kong API Gateway ready

## 🛠️ Quick Start

### Prerequisites

- Node.js 18+
- Docker & Docker Compose (optional)
- Git

### Local Development

```bash
# Clone repository
git clone https://github.com/solnctech-prog/MVP-PRO.git
cd MVP-PRO

# Frontend setup
cd frontend
npm install
npm run dev
# Runs on http://localhost:3000

# Backend setup (new terminal)
cd backend
npm install
npm run dev
# Runs on http://localhost:3001
```

### Docker Compose (Full Stack)

```bash
# Build and run all services
docker-compose up -d

# Services will be available at:
# Frontend:  http://localhost:3000
# Backend:   http://localhost:3001
# Nginx:     http://localhost:80
# Kong Admin: http://localhost:8001
```

## 📁 Project Structure

```
MVP-PRO/
├── frontend/                 # Next.js application
│   ├── src/
│   │   ├── app/             # Pages and layouts
│   │   ├── components/      # React components
│   │   ├── lib/             # Utilities and types
│   │   └── styles/          # CSS files
│   └── package.json
│
├── backend/                  # Express.js server
│   ├── src/
│   │   ├── app.ts          # Express setup
│   │   ├── server.ts       # Server entry point
│   │   ├── routes/         # API routes
│   │   ├── middleware/     # Custom middleware
│   │   └── types/          # TypeScript types
│   └── package.json
│
├── infrastructure/           # Infrastructure configs
│   ├── nginx/              # Nginx configuration
│   ├── kong/               # Kong API Gateway
│   └── docker/             # Docker files
│
└── docker-compose.yml       # Full stack orchestration
```

## 🌐 API Endpoints

### Health Check
```
GET /api/health
Response: { status: 'ok', timestamp: '...', uptime: 123.45 }
```

### Version
```
GET /api/version
Response: { version: '1.0.0', name: 'MVP-PRO API' }
```

## 🔧 Environment Variables

### Frontend (.env.local)
```
NEXT_PUBLIC_API_URL=http://localhost:3001
NEXT_PUBLIC_SITE_URL=http://localhost:3000
NEXT_PUBLIC_COMPANY_NAME=MVP-PRO
```

### Backend (.env.local)
```
NODE_ENV=development
PORT=3001
HOST=0.0.0.0
FRONTEND_URL=http://localhost:3000
API_URL=http://localhost:3001
LOG_LEVEL=debug
```

## 📚 Documentation

- [Architecture Guide](./docs/ARCHITECTURE.md)
- [API Documentation](./docs/API_DOCUMENTATION.md)
- [Deployment Guide](./docs/DEPLOYMENT.md)
- [Development Guide](./docs/DEVELOPMENT.md)

## 🚀 Deployment

### Docker Deployment

```bash
# Build images
docker build -t mvp-pro-frontend:latest ./frontend
docker build -t mvp-pro-backend:latest ./backend

# Run services
docker run -p 3000:3000 mvp-pro-frontend:latest
docker run -p 3001:3001 mvp-pro-backend:latest
```

### Production Checklist

- [ ] Environment variables configured
- [ ] SSL/TLS certificates installed
- [ ] Database configured
- [ ] API rate limiting enabled
- [ ] Monitoring and logging setup
- [ ] Backup strategy in place
- [ ] CI/CD pipeline configured

## 🤝 Contributing

1. Create a feature branch
2. Commit changes
3. Push to branch
4. Create Pull Request

## 📄 License

MIT License - see LICENSE file for details

## 📞 Contact

- Email: support@mvp-pro.tech
- Website: https://mvp-pro.tech
- GitHub: https://github.com/solnctech-prog/MVP-PRO

---

**Built with ❤️ by MVP-PRO Team**
