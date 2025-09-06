# 🍹 Cocktail Machine - Deployment Repository

**Automated deployment releases for Raspberry Pi installations**

This repository contains built, ready-to-deploy packages for the Cocktail Machine system.

## 📦 What's Inside

- **`web/`** - Built dashboard web application
- **`scripts/`** - Installation and update scripts  
- **`kiosk/`** - Kiosk mode configuration files
- **`web/versions.json`** - Version information for update system

## 🚀 For Pi Users

### Quick Installation
```bash
# Download and run the installation script
curl -fsSL https://raw.githubusercontent.com/sebastienlepoder/cocktail-deploy/main/scripts/install.sh | bash
```

### Update Your System
```bash
# Via Node-RED Dashboard (Recommended)
# Go to: http://your-pi-ip:1880/ui → Updates tab → Install Update

# Or via command line
sudo /opt/scripts/update_dashboard.sh
```

## 🔄 Update Methods

1. **Node-RED Dashboard** - Easy web interface
2. **API Endpoint** - `curl -X POST http://pi-ip:1880/api/update/now`  
3. **Update Script** - `sudo /opt/scripts/update_dashboard.sh`
4. **Quick Update** - `sudo bash -c "$(curl -fsSL https://raw.githubusercontent.com/sebastienlepoder/cocktail-deploy/main/scripts/quick-update.sh)"`
5. **Manual Start** - `cd ~/cocktail-machine/deployment && ./start-services.sh`

## 📋 Current Version

Check `web/versions.json` for the latest version information.

## 🔗 Related Repositories

- **[warp-cocktail-machine](https://github.com/sebastienlepoder/warp-cocktail-machine)** - Main development repository
- **[cocktail-machine](https://github.com/sebastienlepoder/cocktail-machine)** - Legacy repository

---

*This repository is automatically updated via GitHub Actions when new releases are built.*
