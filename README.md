# Sports Betting Tracker - Progressive Web App (PWA)

A full-featured Progressive Web App for tracking sports betting trades with offline support, installability, and data persistence.

## 🎯 Features

- **📊 Track Trades**: Record all your betting trades with detailed information
- **📈 Analytics Dashboard**: Visual charts showing performance, win/loss ratios, and profit trends
- **💰 Bankroll Management**: Monitor your bankroll growth over time
- **📅 Monthly View**: Organize and analyze trades by month
- **💾 Data Persistence**: All data saved locally using localStorage
- **📱 Installable**: Add to home screen on mobile and desktop
- **🔌 Offline Support**: Works without internet connection
- **⚡ Fast Loading**: Service worker caching for instant load times

## 📦 Files Included

- `index.html` - Main application file with PWA enhancements
- `manifest.json` - PWA manifest configuration
- `sw.js` - Service worker for offline functionality
- `icon-192.png` - App icon (192x192)
- `icon-512.png` - App icon (512x512)

## 🚀 How to Deploy

### Option 1: GitHub Pages (Free & Easy)

1. Create a new GitHub repository
2. Upload all files to the repository
3. Go to Settings > Pages
4. Select "main" branch and "/" root
5. Click Save
6. Your PWA will be live at `https://yourusername.github.io/repository-name`

### Option 2: Netlify (Free & Easy)

1. Go to [netlify.com](https://netlify.com)
2. Drag and drop the folder containing all files
3. Your PWA will be deployed instantly with HTTPS

### Option 3: Vercel (Free & Easy)

1. Install Vercel CLI: `npm install -g vercel`
2. Navigate to the folder: `cd /path/to/folder`
3. Run: `vercel`
4. Follow the prompts

### Option 4: Local Testing

1. Install a local server:
   ```bash
   npm install -g http-server
   ```
2. Navigate to the folder and run:
   ```bash
   http-server -p 8080
   ```
3. Open `http://localhost:8080` in your browser

**Note**: For PWA features (install prompt, service worker), you need:
- HTTPS connection (required for service workers)
- OR localhost (works for testing)

## 📱 Installing the PWA

### On Mobile (iOS/Android):

1. Open the deployed URL in your browser
2. Look for the "Add to Home Screen" prompt or
3. Tap the share button and select "Add to Home Screen"

### On Desktop (Chrome/Edge):

1. Open the deployed URL
2. Look for the install icon in the address bar or
3. Click the "Install" button when prompted
4. The app will open in its own window

## 🔧 Customization

### Change App Name
Edit `manifest.json`:
```json
"name": "Your App Name",
"short_name": "Short Name"
```

### Change Colors
Edit `manifest.json`:
```json
"theme_color": "#your-color",
"background_color": "#your-color"
```

### Change Starting Bankroll
Edit `index.html`, find:
```javascript
let STARTING_BANKROLL = 1000;
```

### Update Icons
Replace `icon-192.png` and `icon-512.png` with your own icons

## 💾 Data Storage

- All data is stored locally in the browser's localStorage
- Data persists between sessions
- Each browser/device has its own separate data
- To backup data: Use the export feature (if implemented) or copy localStorage manually

## 🛠️ Browser Support

- ✅ Chrome/Edge (full support)
- ✅ Firefox (full support)
- ✅ Safari (full support with some limitations)
- ✅ Opera (full support)

## 📊 PWA Features

### Service Worker
- Caches app resources for offline use
- Enables fast load times
- Provides offline fallback

### Web App Manifest
- Defines app appearance when installed
- Controls display mode (standalone)
- Specifies icons and colors

### LocalStorage
- Persistent data storage
- Survives browser restarts
- No server required

## 🔒 Privacy

- All data stays on your device
- No data is sent to any server
- No tracking or analytics
- Completely private and secure

## 🐛 Troubleshooting

**Install prompt not showing?**
- Ensure you're using HTTPS or localhost
- Clear browser cache and reload
- Check browser console for errors

**Service worker not working?**
- HTTPS is required (except localhost)
- Check browser DevTools > Application > Service Workers
- Unregister old service workers and refresh

**Data not persisting?**
- Check if localStorage is enabled
- Ensure browser isn't in private/incognito mode
- Check browser storage quota

## 📝 License

Free to use and modify as needed.

## 🤝 Support

For issues or questions, check browser console for errors or ensure all files are properly deployed with HTTPS enabled.

---

**Enjoy tracking your betting trades! 🎯💰**
