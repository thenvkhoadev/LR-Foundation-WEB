# LR Foundation WEB - Version 2.0

## 🌹 Tổng Quan

Website Quỹ Bông Hồng Nhỏ (Little Rose Foundation) - Tái cấu trúc hoàn toàn với kiến trúc hiện đại, dễ bảo trì và mở rộng.

## ✨ Tính Năng Mới (v2.0)

### 🏗️ Kiến Trúc
- ✅ **EJS Template Engine**: Thay thế HTML tĩnh bằng template động
- ✅ **Component System**: Header/Footer được quản lý tập trung
- ✅ **Layout System**: Hỗ trợ layouts linh hoạt
- ✅ **Frontend/Backend Tách Biệt**: Cấu trúc rõ ràng hơn

### 🛠️ Build Pipeline
- ✅ **Webpack 5**: Bundle và optimize JavaScript
- ✅ **Tailwind CSS**: Build và purge CSS tự động
- ✅ **PostCSS**: Autoprefixer và optimization
- ✅ **Code Splitting**: Tối ưu load time
- ✅ **Minification**: Tự động nén code trong production

### 📦 JavaScript Organization
- ✅ **ES6 Modules**: Module system hiện đại
- ✅ **Component-based**: Navigation, DarkMode, Animations, Forms
- ✅ **No Global Pollution**: Clean code organization
- ✅ **Event Delegation**: Performance optimization

### 🔒 Security & Performance
- ✅ **Helmet.js**: Security headers
- ✅ **Compression**: Gzip compression
- ✅ **CSP**: Content Security Policy
- ✅ **Lazy Loading**: Images và resources

## 📁 Cấu Trúc Dự Án (Mới)

```
LR-Foundation-WEB/
├── src/
│   ├── assets/                  # Frontend assets
│   │   ├── css/
│   │   │   └── index.css        # Tailwind base + custom styles
│   │   └── images/              # Image assets
│   ├── components/              # React Components
│   │   ├── features/            # Feature-specific components
│   │   │   ├── admin/          # Admin dashboard components
│   │   │   ├── auth/           # Authentication components
│   │   │   ├── donation/       # Donation form & tracking
│   │   │   ├── news/           # News/blog components
│   │   │   └── programs/       # Program showcase
│   │   ├── layout/             # Layout components
│   │   │   ├── Header.tsx      # Navigation header
│   │   │   ├── Footer.tsx      # Site footer
│   │   │   ├── Sidebar.tsx     # Admin sidebar
│   │   │   └── Layout.tsx      # Main layout wrapper
│   │   ├── ui/                 # Reusable UI components
│   │   │   ├── Button.tsx      # Button variants
│   │   │   ├── Card.tsx        # Card component
│   │   │   ├── Input.tsx       # Form inputs
│   │   │   ├── Modal.tsx       # Modal dialogs
│   │   │   └── Loading.tsx     # Loading states
│   │   └── Toast.tsx           # Toast notifications
│   ├── pages/                  # Route pages
│   │   ├── Home.tsx            # Landing page
│   │   ├── About.tsx           # About organization
│   │   ├── Programs.tsx        # Programs listing
│   │   ├── News.tsx            # News/blog page
│   │   ├── Donate.tsx          # Donation page
│   │   ├── Contact.tsx         # Contact form
│   │   ├── Finance.tsx         # Financial transparency
│   │   └── admin/              # Admin pages
│   │       ├── Dashboard.tsx
│   │       ├── Users.tsx
│   │       └── Settings.tsx
│   ├── hooks/                  # Custom React hooks
│   │   ├── useAuth.ts          # Authentication hook
│   │   ├── useDarkMode.ts      # Dark mode toggle
│   │   ├── useToast.ts         # Toast notifications
│   │   └── useApi.ts           # API calls wrapper
│   ├── services/               # API services
│   │   ├── api.ts              # Axios instance
│   │   ├── authService.ts      # Auth API calls
│   │   ├── donationService.ts  # Donation API
│   │   └── newsService.ts      # News API
│   ├── types/                  # TypeScript definitions
│   │   ├── index.ts            # Common types
│   │   ├── user.types.ts       # User types
│   │   ├── donation.types.ts   # Donation types
│   │   └── api.types.ts        # API response types
│   ├── utils/                  # Utility functions
│   │   ├── helpers.ts          # Helper functions
│   │   ├── validators.ts       # Form validation
│   │   └── formatters.ts       # Data formatters
│   ├── config/                 # Configuration
│   │   ├── constants.ts        # App constants
│   │   └── theme.ts            # Theme configuration
│   ├── App.tsx                 # Root component
│   ├── main.tsx                # Application entry point
│   ├── index.css               # Global styles
│   ├── vite-env.d.ts           # Vite type definitions
│   └── README.md               # Source code documentation
│
├── public/                     # Static assets
│   ├── clear-storage.html      # Storage utility page
│   └── images/                 # Public images
│       └── images/             # Image subdirectory
│
├── .qodo/                      # Qodo AI configuration
│   ├── agents/                 # AI agents
│   └── workflows/              # Automation workflows
│
├── .env.example                # Environment variables template
├── .env copy.example           # Backup env template
├── .gitignore                  # Git ignore rules
├── .gitignore copy             # Backup gitignore
├── About.tsx                   # About page component (root level)
├── eslint.config.js            # ESLint configuration
├── index.html                  # HTML entry point
├── LICENSE                     # License file
├── package.json                # Dependencies & scripts
├── postcss.config.js           # PostCSS configuration
├── README.md                   # Project documentation
├── tailwind.config.js          # Tailwind CSS configuration
├── tsconfig.app.json           # TypeScript app config
├── tsconfig.json               # TypeScript base config
├── tsconfig.node.json          # TypeScript Node config
├── vercel.json                 # Vercel deployment config
└── vite.config.ts              # Vite build configuration
```

## 🚀 Cài Đặt

### Yêu Cầu
- Node.js >= 18.0.0
- npm hoặc yarn

### Bước 1: Clone Repository
```bash
git clone https://github.com/hayamij/LR-Foundation-WEB.git
cd LR-Foundation-WEB
```

### Bước 2: Cài Đặt Dependencies
```bash
npm install
```

### Bước 3: Build Assets
```bash
npm run build
```

### Bước 4: Chạy Development Server
```bash
npm run dev
```

Server sẽ chạy tại: http://localhost:3000

## 📝 Scripts

```bash
# Development mode (hot reload)
npm run dev

# Build production assets
npm run build

# Start production server
npm start

# Build CSS only
npm run build:css

# Watch CSS changes
npm run watch:css
```

## 🔧 Công Nghệ Sử Dụng

### Backend
- **Express.js** - Web framework
- **EJS** - Template engine
- **Helmet** - Security middleware
- **Compression** - Response compression

### Frontend
- **Tailwind CSS** - Utility-first CSS
- **Vanilla JavaScript** - ES6+ modules
- **Material Icons** - Icon library

### Build Tools
- **Webpack 5** - Module bundler
- **PostCSS** - CSS processor
- **Autoprefixer** - CSS vendor prefixing
- **Terser** - JavaScript minifier

### Development
- **Nodemon** - Auto-restart server
- **npm-run-all** - Run multiple scripts

## 🎨 Customization

### Thay Đổi Theme Colors
Edit `tailwind.config.js`:
```javascript
theme: {
  extend: {
    colors: {
      primary: '#2A7050',
      secondary: '#B12029',
      // Add your colors...
    }
  }
}
```

### Thêm Custom CSS
Edit `src/assets/css/input.css`:
```css
@layer components {
  .your-custom-class {
    /* Your styles */
  }
}
```

### Thêm JavaScript Module
Create file trong `src/assets/js/modules/` và import vào `index.js`

## 🔍 So Sánh v1.0 vs v2.0

| Tính năng | v1.0 | v2.0 |
|-----------|------|------|
| Template Engine | ❌ Static HTML | ✅ EJS Dynamic |
| Component Management | ❌ Fetch-based | ✅ Server-side includes |
| CSS Build | ❌ CDN | ✅ Tailwind Build |
| JS Organization | ❌ Global scope | ✅ ES6 Modules |
| Build Pipeline | ❌ None | ✅ Webpack |
| Code Splitting | ❌ None | ✅ Automatic |
| CSS Purging | ❌ None | ✅ Automatic |
| Security Headers | ❌ None | ✅ Helmet |
| Compression | ❌ None | ✅ Gzip |

## 📚 Tài Liệu Thêm

- [Express.js Documentation](https://expressjs.com/)
- [EJS Documentation](https://ejs.co/)
- [Tailwind CSS Documentation](https://tailwindcss.com/)
- [Webpack Documentation](https://webpack.js.org/)

## 🤝 Đóng Góp

Mọi đóng góp đều được chào đón! Vui lòng:
1. Fork repository
2. Tạo branch mới (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Mở Pull Request

## 📄 License

MIT License - Xem file [LICENSE](LICENSE) để biết thêm chi tiết

## 👥 Team

LR Foundation Team - [@hayamij](https://github.com/hayamij) & [@thenvkhoadev](https://github.com/thenvkhoadev)

## 🌟 Acknowledgments

- Tailwind CSS team
- Express.js community
- All contributors and supporters

---

Made with ❤️ for Vietnamese children
