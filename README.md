# 🌐 AutoFT Bot Wildcard

<div align="center">

[![npm version](https://badge.fury.io/js/autoft-bot-wildcard.svg)](https://www.npmjs.com/package/autoft-bot-wildcard)
[![Downloads](https://img.shields.io/npm/dm/autoft-bot-wildcard.svg)](https://www.npmjs.com/package/autoft-bot-wildcard)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Node.js](https://img.shields.io/badge/Node.js-20%2B-green.svg)](https://nodejs.org/)

**🚀 Advanced Telegram Bot for Automated Cloudflare Wildcard Domain Management**

**⭐ If this project is useful for you, please give it a star!**  
**🍴 Feel free to fork and contribute!**

[📦 NPM Package](https://www.npmjs.com/package/autoft-bot-wildcard) • [📢 Updates Channel](https://t.me/AutoFtFile) • [🐛 Issues](https://github.com/AutoFTbot/Wildcard-Bot/issues)

</div>

---

## ⚡ Quick Setup

### 1️⃣ Install Package

```bash
npm install -g autoft-bot-wildcard
```

### 2️⃣ Run Interactive Setup

```bash
autoft-bot-wildcard
```

### 3️⃣ Start Your Bot

```bash
cd autoft-bot-wildcard
npm start
```

**🎉 Your bot is now live and ready!**

---

## 🚀 Production Setup with PM2

### Install PM2 & Setup Service

```bash
# Install PM2 globally
npm install -g pm2

# Navigate to your bot directory
cd autoft-bot-wildcard

# Start bot with PM2
pm2 start index.js --name "autoft-bot-wildcard"

# Save PM2 configuration
pm2 save

# Enable auto-start on system boot
pm2 startup

# Check status
pm2 status
```

### PM2 Management Commands

```bash
# Monitor logs
pm2 logs autoft-bot-wildcard

# Restart bot
pm2 restart autoft-bot-wildcard

# Stop bot
pm2 stop autoft-bot-wildcard

# Delete from PM2
pm2 delete autoft-bot-wildcard

# Monitor all processes
pm2 monit
```

---

## ✨ Features

<div align="center">

| 🤖 **Bot Interface** | 🌐 **Cloudflare** | 👥 **Multi-User** | 🔐 **Secure** |
|:---:|:---:|:---:|:---:|
| Complete Telegram management | Automated DNS setup | Individual domain control | Safe API storage |

| 📊 **Analytics** | 📢 **Notifications** | 🎨 **Easy Setup** | ⚡ **Performance** |
|:---:|:---:|:---:|:---:|
| Real-time statistics | Instant Telegram alerts | Interactive CLI wizard | Lightweight & fast |

</div>

---

## 🎯 Quick Commands

### 🔰 Basic Usage
```bash
/start                           # Start the bot
/addcf <api_key> <email>        # Add Cloudflare credentials
/listdomain                      # Show available domains
/setupwildcard example.com       # Setup wildcard domain
/mysub                          # View your subdomains
```

### 👑 Admin Commands
```bash
/stats                          # Bot statistics
/broadcast <message>            # Send to all users
/userinfo <user_id>            # User details
/testnotif                     # Test notifications
```

---

## ⚙️ Configuration

### Required Environment

- **Node.js 20+** - [Download here](https://nodejs.org/)
- **Telegram Bot Token** - Get from [@BotFather](https://t.me/BotFather)
- **Cloudflare Account** - [Sign up here](https://cloudflare.com/)

### Environment Variables

```env
# 🤖 Bot Configuration
BOT_TOKEN=your_bot_token_here
ADMIN_IDS=123456789

# 📢 Optional: Notifications
TELEGRAM_GROUP_ID=-1001234567890

# 🔧 Optional: Settings
MAX_CUSTOM_DOMAINS=5
NODE_ENV=production
```

---

## 📚 Documentation

<div align="center">

| 📖 **Guide** | 🔧 **Setup** | 🆘 **Help** | 🚀 **Start** |
|:---:|:---:|:---:|:---:|
| [Commands](wiki/Commands.md) | [Configuration](wiki/Configuration.md) | [Troubleshooting](wiki/Troubleshooting.md) | [Quick Start](wiki/Quick-Start.md) |

[🏠 **Complete Wiki**](wiki/Home.md)

</div>

---

## 💝 Support the Project

<div align="center">

### 💰 Donate via QRIS (Indonesia)

![QRIS Donation](https://raw.githubusercontent.com/AutoFTbot/AutoFTbot/refs/heads/main/assets/QRIS.jpg)

**Your donation helps us maintain and improve this project!**

### 🌟 Other Ways to Support

[![Star](https://img.shields.io/badge/⭐-Star%20this%20repo-yellow?style=for-the-badge)](https://github.com/AutoFTbot/Wildcard-Bot)
[![Fork](https://img.shields.io/badge/🍴-Fork%20&%20Share-blue?style=for-the-badge)](https://github.com/AutoFTbot/Wildcard-Bot/fork)
[![Issues](https://img.shields.io/badge/🐛-Report%20Bugs-red?style=for-the-badge)](https://github.com/AutoFTbot/Wildcard-Bot/issues)

</div>

---

## 📊 Project Stats

<div align="center">

![GitHub stars](https://img.shields.io/github/stars/AutoFTbot/Wildcard-Bot.svg?style=social&label=Star)
![GitHub forks](https://img.shields.io/github/forks/AutoFTbot/Wildcard-Bot.svg?style=social&label=Fork)
![GitHub watchers](https://img.shields.io/github/watchers/AutoFTbot/Wildcard-Bot.svg?style=social&label=Watch)

![GitHub repo size](https://img.shields.io/github/repo-size/AutoFTbot/Wildcard-Bot)
![GitHub commit activity](https://img.shields.io/github/commit-activity/m/AutoFTbot/Wildcard-Bot)
![NPM Downloads](https://img.shields.io/npm/dt/autoft-bot-wildcard)

</div>

---

## 📞 Support & Community

<div align="center">

[![Telegram Channel](https://img.shields.io/badge/📢%20Updates-Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/AutoFtFile)
[![GitHub Issues](https://img.shields.io/badge/🐛%20Issues-GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/AutoFTbot/Wildcard-Bot/issues)
[![Developer](https://img.shields.io/badge/👨‍💻%20Developer-Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/AutoFtBot69)

</div>

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🌐 Web Dashboard (Coming Soon)

<div align="center">

### 🎨 Modern Web Interface

**Manage your wildcard domains from anywhere with our upcoming web dashboard!**

![Web Dashboard Preview](https://via.placeholder.com/800x400/2ea44f/ffffff?text=AutoFT+Web+Dashboard+Coming+Soon)

</div>

### 🚀 Planned Features

<div align="center">

| 📊 **Analytics** | 🎛️ **Control Panel** | 👥 **User Management** | 🔔 **Notifications** |
|:---:|:---:|:---:|:---:|
| Real-time domain stats | Drag & drop interface | Role-based access | Live activity feed |
| Traffic monitoring | Bulk operations | Team collaboration | Custom alerts |
| Performance insights | Quick actions | Permission controls | Email & Telegram |

</div>

### 🛠️ Tech Stack

```javascript
// Modern web technologies planned
{
  "frontend": ["React", "Next.js", "TailwindCSS", "Chart.js"],
  "backend": ["Node.js", "Express", "Socket.io", "JWT"],
  "database": ["MongoDB", "Redis"],
  "deployment": ["Docker", "Nginx", "PM2"]
}
```

### 🎯 Web Features Roadmap

- [ ] 🎨 **Q2 2024**: Modern dashboard UI/UX
- [ ] 📊 **Q2 2024**: Real-time analytics & charts  
- [ ] 👥 **Q3 2024**: Multi-user management portal
- [ ] 🔐 **Q3 2024**: Advanced security & 2FA
- [ ] 📱 **Q4 2024**: Mobile-responsive design
- [ ] 🌍 **Q4 2024**: Multi-language support
- [ ] 🔗 **2025**: REST API & webhooks
- [ ] ⚡ **2025**: GraphQL integration

### 💡 Sneak Peek

<div align="center">

**🎛️ Dashboard Overview**
```
┌─────────────────────────────────────────────────┐
│  AutoFT Web Dashboard                     🔔 📊 │
├─────────────────────────────────────────────────┤
│  📈 Analytics    🌐 Domains    👥 Users    ⚙️   │
├─────────────────────────────────────────────────┤
│                                                 │
│  🎯 Quick Actions                               │
│  ┌─────────────┐ ┌─────────────┐ ┌───────────┐  │
│  │ Add Domain  │ │ Setup Wild  │ │ View Logs │  │
│  │     +       │ │     *.     │ │    📋    │  │
│  └─────────────┘ └─────────────┘ └───────────┘  │
│                                                 │
│  📊 Domain Statistics                           │
│  ┌─ example.com ────────────────── 89% ──┐     │
│  ┌─ demo.net ──────────────────── 76% ──┐      │
│  ┌─ test.org ──────────────────── 45% ──┐      │
│                                                 │
└─────────────────────────────────────────────────┘
```

</div>

### 🎪 Interactive Demo

Want early access to the web dashboard? Join our beta program!

<div align="center">

[![Beta Access](https://img.shields.io/badge/🌟-Join%20Beta%20Program-ff6b6b?style=for-the-badge)](https://t.me/AutoFtFile)
[![Web Demo](https://img.shields.io/badge/🌐-View%20Demo-4ecdc4?style=for-the-badge)](https://demo.autoft-bot.com)

**📢 Get notified when web dashboard launches!**

</div>

---

## 👨‍💻 For Developers

<div align="center">

**Join our development team and help build the future of domain management!**

</div>

### 🚀 Development Stack

```bash
# Current Bot Architecture
├── 🤖 Telegram Bot (Node.js + Telegraf)
├── ☁️ Cloudflare API Integration  
├── 📊 Real-time Analytics
└── 🔧 PM2 Process Management

# Upcoming Web Stack
├── ⚛️ Frontend (React + Next.js + TailwindCSS)
├── 🗄️ Backend (Node.js + Express + Socket.io)
├── 💾 Database (MongoDB + Redis)
└── 🐳 DevOps (Docker + Nginx + GitHub Actions)
```

### 🛠️ Contributing Areas

<div align="center">

| 🎨 **Frontend** | 🔧 **Backend** | 📱 **Mobile** | 🧪 **Testing** |
|:---:|:---:|:---:|:---:|
| React/Next.js | Node.js/Express | React Native | Jest/Cypress |
| UI/UX Design | API Development | iOS/Android | Performance |
| Dashboard | Database Design | PWA | Security |

</div>

### 🎯 Open Opportunities

- 🎨 **UI/UX Designer** - Design the web dashboard interface
- ⚛️ **React Developer** - Build responsive frontend components  
- 🔧 **Backend Developer** - API & database architecture
- 📱 **Mobile Developer** - React Native mobile app
- 🧪 **QA Engineer** - Testing & automation
- 📝 **Technical Writer** - Documentation & tutorials
- 🌍 **Translator** - Multi-language support

### 💡 Quick Start Development

```bash
# Clone the repository
git clone https://github.com/AutoFTbot/Wildcard-Bot.git
cd Wildcard-Bot

# Install dependencies
npm install

# Set up development environment
cp .env.example .env.dev
nano .env.dev

# Start development mode
npm run dev

# Run tests
npm test

# Build for production
npm run build
```

### 🏆 Contributor Benefits

- 🌟 **Recognition** in project credits
- 📈 **Portfolio** enhancement with real-world project
- 🤝 **Networking** with global developer community
- 🎓 **Learning** modern web technologies
- 💰 **Revenue sharing** for premium features (planned)

<div align="center">

[![Contribute](https://img.shields.io/badge/🚀-Start%20Contributing-success?style=for-the-badge)](https://github.com/AutoFTbot/Wildcard-Bot/blob/main/CONTRIBUTING.md)
[![Discord](https://img.shields.io/badge/💬-Developer%20Chat-7289DA?style=for-the-badge&logo=discord)](https://discord.gg/autoft-dev)

</div>

---

<div align="center">

**🌟 If this project helped you, please consider giving it a star!**

**Made with ❤️ by the AutoFTbot Team**  
**Developer: [@AutoFtBot69](https://t.me/AutoFtBot69)**

[🚀 **Get Started Now**](https://www.npmjs.com/package/autoft-bot-wildcard) • [📢 **Updates Channel**](https://t.me/AutoFtFile) • [💰 **Donate**](https://raw.githubusercontent.com/AutoFTbot/AutoFTbot/refs/heads/main/assets/QRIS.jpg)

</div>
