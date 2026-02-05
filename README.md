# CSE Lab Finder - Spring 2026

Find available CSE labs instantly! This tool helps students check lab availability across different time slots and days.

## 🚀 Features

- **Real-time Lab Availability**: Check if labs are free or occupied
- **Smart Filtering**: Filter by day and time slot
- **Beautiful UI**: Modern, responsive design with smooth animations
- **Detailed Information**: See which courses are ongoing with faculty info
- **Mobile Friendly**: Works perfectly on all devices

## 📦 Deployment Instructions

### Deploy to Vercel (Recommended)

1. **Install Vercel CLI** (if not already installed):
   ```bash
   npm install -g vercel
   ```

2. **Navigate to project folder**:
   ```bash
   cd your-project-folder
   ```

3. **Deploy**:
   ```bash
   vercel
   ```

4. Follow the prompts and your site will be live!

### Alternative: Deploy via Vercel Dashboard

1. Go to [vercel.com](https://vercel.com)
2. Sign in with GitHub/GitLab/Bitbucket
3. Click "New Project"
4. Import your repository or drag & drop the project folder
5. Click "Deploy"
6. Your site will be live in seconds!

### GitHub Pages Deployment

1. Push the files to a GitHub repository
2. Go to Settings → Pages
3. Select the branch to deploy
4. Your site will be live at `https://username.github.io/repository-name`

## 📁 Project Structure

```
.
├── index.html       # Main HTML file
├── script.js        # JavaScript logic with lab data
├── vercel.json      # Vercel configuration
├── package.json     # Project metadata
└── README.md        # This file
```

## 🛠️ Local Development

Simply open `index.html` in your browser - no build process needed!

Or use a local server:
```bash
# Python 3
python -m http.server 8000

# Node.js (install http-server first: npm install -g http-server)
http-server

# Then visit http://localhost:8000
```

## 🔧 Customization

To update lab schedules:
1. Open `script.js`
2. Find the `labSchedule` object
3. Add/modify lab entries following the existing format
4. Save and redeploy

## 📝 Lab Data Format

```javascript
"LAB-ROOM": [
    { 
        course: "COURSE-CODE", 
        faculty: "FACULTY-INITIALS", 
        day: "DAY", 
        time: "TIME" 
    }
]
```

## 💻 Prepared By

**IMPOSTER SERVER TEAM**

Making student life easier, one lab at a time! 🚀

## 📄 License

MIT License - Feel free to use and modify!

## 🐛 Issues?

If you encounter any issues:
1. Make sure all files are in the same directory
2. Check browser console for errors (F12)
3. Ensure JavaScript is enabled
4. Try a different browser

## 🎯 Troubleshooting Vercel Deployment

If deployment fails:

1. **Check file structure**: Ensure `index.html` is in root directory
2. **Verify vercel.json**: Should be in root directory
3. **Clear build cache**: Run `vercel --force`
4. **Check logs**: Use `vercel logs [deployment-url]`

Common fixes:
```bash
# Remove node_modules if exists
rm -rf node_modules

# Clear Vercel cache
vercel --force

# Redeploy
vercel --prod
```

## 📱 Contact

For updates and support, reach out to **IMPOSTER SERVER TEAM**

---

Made with ❤️ for CSE students
