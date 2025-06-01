# 🌐 Auto Wildcard Telegram Bot

[![npm version](https://badge.fury.io/js/auto-wildcard-domain-bot.svg)](https://www.npmjs.com/package/auto-wildcard-domain-bot)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Node.js](https://img.shields.io/badge/Node.js-20%2B-green.svg)](https://nodejs.org/)

**The easiest way to set up a Telegram Bot for Cloudflare Wildcard Domain Management!**

🚀 **Just 3 commands and you're ready!**

## ⚡ Quick Start (Under 2 minutes!)

### 1. Install globally

```bash
npm install -g auto-wildcard-domain-bot
```

### 2. Run interactive setup

```bash
auto-wildcard-domain-bot
```

### 3. Start your bot

```bash
cd auto-wildcard-domain-bot
npm start
```

**That's it!** 🎉 Your bot is now running and ready to manage wildcard domains!

---

## 📋 What you get

✅ **Complete Telegram Bot** - Ready to use, no coding required  
✅ **Cloudflare Integration** - Automatic wildcard domain setup  
✅ **Admin Dashboard** - Monitor users and domains  
✅ **Custom Domains** - Let users add their own subdomains  
✅ **Analytics** - Track domain performance

## 🔧 Prerequisites (Only 2 things!)

1. **Node.js 20+** - [Download here](https://nodejs.org/)
2. **Telegram Bot Token** - Get from [@BotFather](https://t.me/BotFather)

That's all you need! The setup wizard will guide you through everything else.

## 📱 Interactive Setup

When you run `auto-wildcard-domain-bot`, you'll get a beautiful interactive setup:

```
🌐 AUTO WILDCARD TELEGRAM BOT SETUP
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Welcome! Let's set up your Auto Wildcard Telegram Bot in 3 easy steps:
  1️⃣  Bot Token Configuration
  2️⃣  Admin Setup
  3️⃣  Launch Bot

1️⃣  BOT TOKEN CONFIGURATION
ℹ Get your bot token from @BotFather on Telegram
ℹ Link: https://t.me/BotFather

Enter your bot token:
```

The setup wizard will:

- ✅ Validate your bot token
- ✅ Set up admin permissions
- ✅ Create all necessary config files
- ✅ Install dependencies automatically
- ✅ Provide clear next steps

## 🎯 User Experience

### For Bot Users (Your Customers)

Your users get access to powerful commands:

```
/start          - Welcome & setup guide
/addcf          - Add Cloudflare credentials
/setupwildcard  - Setup wildcard domain
/listdomain     - View available domains
/new            - Add custom subdomain
/analytics      - View domain stats
```

### For You (Bot Owner)

You get admin-only features:

```
/stats       - Bot usage statistics
/broadcast   - Send message to all users
/userinfo    - View user details
/testnotif   - Test notification system
```

## 🏗️ What gets created

When you run `auto-wildcard-domain-bot`, it creates a clean project structure:

```
auto-wildcard-domain-bot/
├── .env                 # Your bot configuration
├── config/default.js    # Bot settings
├── package.json         # Project info
├── index.js            # Main bot file
└── data/               # Bot data storage
```

**Everything is pre-configured and ready to run!**

## 🔧 Advanced Usage

### Programmatic Usage

You can also use this as a library in your own projects:

```javascript
const WildcardBot = require('auto-wildcard-domain-bot');

const bot = new WildcardBot({
    configPath: './my-config.js',
    dataPath: './my-data',
});

bot.start();
```

### Custom Configuration

Modify `config/default.js` to customize:

```javascript
module.exports = {
    ADMIN_IDS: [123456789], // Your Telegram ID
    MAX_CUSTOM_DOMAINS: 10, // Limit per user
    DEFAULT_DOMAINS: ['yourdomain.com'], // Available domains

    NOTIFICATIONS: {
        TELEGRAM: { enabled: true },
        WHATSAPP: { enabled: false }, // Optional WhatsApp alerts
    },
};
```

## 📊 Features in Detail

### 🌐 Wildcard Domain Management

- Automatic Cloudflare Worker deployment
- DNS record creation and management
- SSL certificate handling
- Subdomain routing

### 📲 Smart Notifications

- **Telegram Groups**: Real-time admin alerts
- **Privacy-aware**: Censored domains in public channels

### 👑 Admin Controls

- User statistics and analytics
- Broadcast messaging system
- Individual user management
- System health monitoring

### 🛡️ Security Features

- Admin-only command restrictions
- Input validation and sanitization
- Rate limiting and spam protection
- Secure credential storage

## 🚀 Production Ready

Your bot comes production-ready with:

- ✅ Error handling and recovery
- ✅ Graceful shutdown handling
- ✅ File-based data persistence
- ✅ Comprehensive logging
- ✅ PM2 support for process management

### Deploy with PM2

```bash
npm install -g pm2
pm2 start index.js --name "auto-wildcard-domain-bot"
pm2 startup
pm2 save
```

## 📖 Commands Reference

### 🔰 Basic Commands

| Command  | Description                | Usage    |
| -------- | -------------------------- | -------- |
| `/start` | Welcome message & bot info | `/start` |
| `/help`  | Full command guide         | `/help`  |

### 🔧 Configuration

| Command     | Description                | Usage                         |
| ----------- | -------------------------- | ----------------------------- |
| `/addcf`    | Add Cloudflare credentials | `/addcf <api_key> <email>`    |
| `/cfconfig` | View your config           | `/cfconfig`                   |
| `/updatecf` | Update credentials         | `/updatecf <api_key> <email>` |
| `/deletecf` | Remove config              | `/deletecf`                   |

### 🌐 Domain Management

| Command          | Description           | Usage                     |
| ---------------- | --------------------- | ------------------------- |
| `/setupwildcard` | Setup wildcard domain | `/setupwildcard <domain>` |
| `/listdomain`    | Available domains     | `/listdomain`             |
| `/new`           | Add custom subdomain  | `/new <subdomain>`        |
| `/mysub`         | Your subdomains       | `/mysub`                  |

### 📊 Analytics & Tools

| Command       | Description            | Usage                  |
| ------------- | ---------------------- | ---------------------- |
| `/analytics`  | Domain statistics      | `/analytics <domain>`  |
| `/clearcache` | Clear Cloudflare cache | `/clearcache <domain>` |

### 👑 Admin Commands

| Command      | Description        | Usage                  |
| ------------ | ------------------ | ---------------------- |
| `/stats`     | Bot statistics     | `/stats`               |
| `/broadcast` | Message all users  | `/broadcast <message>` |
| `/testnotif` | Test notifications | `/testnotif`           |
| `/userinfo`  | User details       | `/userinfo <user_id>`  |

## 🔧 Troubleshooting

### Common Issues

**Bot not responding?**

```bash
# Check if bot is running
ps aux | grep node

# Check logs
tail -f ~/.pm2/logs/auto-wildcard-domain-bot-out.log
```

**Can't find auto-wildcard-domain-bot command?**

```bash
# Make sure global install worked
npm list -g auto-wildcard-domain-bot

# Or install locally and run
npx auto-wildcard-domain-bot
```

**Configuration issues?**

```bash
# Re-run setup
auto-wildcard-domain-bot

# Or manually edit
nano auto-wildcard-domain-bot/.env
```

## 💡 Tips & Best Practices

1. **Keep your bot token secure** - Never share it publicly
2. **Set up notifications** - Stay informed about domain setups
3. **Regular backups** - Backup your `data/` directory
4. **Monitor usage** - Use `/stats` to track bot activity
5. **Update regularly** - Keep your NPM package updated

## 🆘 Need Help?

- 💬 **Telegram**: [@AutoFtBot69](https://t.me/AutoFtBot69)
- 🐛 **Issues**: [GitHub Issues](https://github.com/AutoFTbot/Wildcard-Bot/issues)
- 📖 **Wiki**: [Documentation](https://github.com/AutoFTbot/Wildcard-Bot/wiki)

## 📄 License

MIT License - see [LICENSE](LICENSE) file for details.

---

<div align="center">

**⭐ Star this repo if it helped you!**

Made with ❤️ for the community

[🚀 Get Started](https://www.npmjs.com/package/auto-wildcard-domain-bot) • [📖 Documentation](https://github.com/AutoFTbot/Wildcard-Bot) • [💬 Support](https://t.me/AutoFtBot69)

</div>

## ✨ Features

🎯 **Core Functions:**

- ✅ **Setup Wildcard** - Automated Cloudflare wildcard domain configuration
- ✅ **Domain Management** - Complete subdomain control via Telegram
- ✅ **Multi-User Support** - Each user gets their personal domain space
- ✅ **Smart Analytics** - Real-time domain statistics and insights
- ✅ **Cache Control** - Advanced Cloudflare cache management
- ✅ **Admin Panel** - Comprehensive bot management interface
- ✅ **Telegram Notifications** - Get alerts on domain setup

🔧 **Technical Features:**

- ✅ **NPM Package** - Easy global installation
- ✅ **Environment Config** - Secure API key management
- ✅ **Rate Limiting** - Built-in abuse protection
- ✅ **Error Handling** - Comprehensive error reporting
- ✅ **Auto-Setup** - Interactive configuration wizard
- ✅ **CLI Tools** - Command-line utilities

## 🚀 Quick Setup

```bash
# Install globally
npm install -g auto-wildcard-domain-bot

# Run interactive setup
auto-wildcard-domain-bot

# Or manual setup:
git clone https://github.com/AutoFTbot/Wildcard-Bot.git
cd auto-wildcard-domain-bot
npm install
npm start
```

### 📋 Environment Variables

Create `.env` file in your project root:

```env
# Bot Configuration
BOT_TOKEN=your_telegram_bot_token
ADMIN_IDS=123456789,987654321

# Telegram Notifications
TELEGRAM_GROUP_ID=your_telegram_group_id

# Optional Settings
MAX_CUSTOM_DOMAINS=5
NODE_ENV=production
```

## 📱 Notification Setup

```javascript
// config/default.js
NOTIFICATIONS: {
    TELEGRAM: {
        enabled: true,
        groupId: process.env.TELEGRAM_GROUP_ID || '',
    },
},
```

## 🛠️ Development

- **Telegram Bot API**: Real-time bot interactions
- **Node.js & NPM**: Core runtime and package management
- **Cloudflare API**: Domain and DNS management
- **Rate Limiting**: Built-in request throttling

## 🔒 Security & Anti-Piracy Protection

Package ini dilindungi dengan beberapa layer security:

### 1. Code Obfuscation
- Source code utama telah di-obfuscate untuk mencegah reverse engineering
- Variabel dan function names telah dienkripsi
- Control flow protection untuk mempersulit analisis

### 2. License Protection
Package ini dilisensikan dengan **Custom Proprietary License**:
- ✅ Penggunaan untuk tujuan personal dan educational
- ❌ **DILARANG** untuk:
  - Modifikasi dan redistribusi
  - Penggunaan komersial tanpa izin
  - Reverse engineering
  - Pembuatan karya turunan

### 3. Runtime Verification
- Verifikasi integritas package saat runtime
- Detection terhadap unauthorized modification
- Automatic reporting untuk suspicious activity

### 4. Watermarking
Setiap instance bot memiliki watermark unik:
```
🤖 Powered by AutoWildcard Bot v2.0
📧 Contact: @AutoFtBot69
⚠️  Licensed Software - Unauthorized use prohibited
```

### 5. Usage Tracking
- Anonymous usage analytics untuk monitoring
- Detection pattern untuk commercial usage
- Automated license compliance checking

## ⚖️ Legal Notice

**PERINGATAN HUKUM:**
- Penggunaan tidak sah dari software ini dapat berakibat tindakan hukum
- Pelanggaran license akan dilaporkan ke platform terkait
- Kami menggunakan digital fingerprinting untuk tracking unauthorized usage

Dengan menggunakan package ini, Anda setuju untuk:
1. Mematuhi semua ketentuan license
2. Tidak melakukan reverse engineering
3. Tidak mendistribusikan ulang tanpa izin
4. Menggunakan hanya untuk tujuan yang diizinkan

## 📞 Support & Licensing

Untuk pertanyaan licensing atau penggunaan komersial:
- Telegram: [@AutoFtBot69](https://t.me/AutoFtBot69)
- Email: licensing@autowildcard.com
