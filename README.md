# 🍹 Cocktail Machine - Production Release

**Latest Version:** `v2025.09.07-major-7bc487c`  
**Release Type:** major  
**Released:** 2025-09-07T04:02:12Z  
**From Dev Repo:** [sebastienlepoder/cocktail-machine](https://github.com/sebastienlepoder/cocktail-machine)

## 🚀 For Pi Users

### Quick Installation
```bash
curl -fsSL https://raw.githubusercontent.com/sebastienlepoder/cocktail-deploy/main/scripts/setup-ultimate.sh | bash
```

### Update Your System
```bash
# Via Node-RED Dashboard (Recommended)
# Go to: http://your-pi-ip:1880/ui → Updates tab → Install Update

# Or via command line
sudo /opt/scripts/update_dashboard.sh
```

## 📋 Release Notes

🎉 COMPLETE SYSTEM REWRITE! Fresh Pi installations now download your React dashboard directly from production. No more old Next.js dashboard! Setup script completely rewritten to use production repo, correct Docker config, working kiosk mode. This is a MAJOR update - fresh installs will work perfectly out of the box.

## 🔄 Update Methods

1. **Node-RED Dashboard** - Easy web interface at `http://pi-ip:1880/ui`
2. **API Endpoint** - `curl -X POST http://pi-ip:1880/api/update/now`  
3. **Update Script** - `sudo /opt/scripts/update_dashboard.sh`
4. **Quick Update** - `sudo bash -c "$(curl -fsSL https://raw.githubusercontent.com/sebastienlepoder/cocktail-deploy/main/scripts/quick-update.sh)"`
5. **Manual Start** - `cd ~/cocktail-machine/deployment && ./start-services.sh`

## 📦 Contents

- **`web/`** - Dashboard application (version v2025.09.07-major-7bc487c)
- **`scripts/`** - Installation and update scripts  
- **`kiosk/`** - Kiosk mode configuration
- **`web.tar.gz`** - Compressed deployment archive

---

*🤖 Automatically deployed from dev repository via GitHub Actions*  
*⏰ Last updated: 2025-09-07T04:02:12Z*
