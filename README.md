# A.M.A Selections Investor Dashboard

## 📁 File Structure for GitHub Upload

Upload these files to your GitHub repository:

### Root Directory Files:
- `package.json`
- `vite.config.js`
- `index.html`
- `ama-selections-data.csv`
- `README.md` (this file - optional)

### Create `src` folder and upload:
- `main.jsx`
- `investor-dashboard.jsx`

## 🚀 Vercel Deployment

Once all files are uploaded to GitHub:
1. Go to vercel.com
2. Import your repository
3. Deploy!

## ⚙️ Configuration Required

Before deploying, you must update the CONFIG section in `src/investor-dashboard.jsx`:

```javascript
const CONFIG = {
  GOOGLE_SHEETS_API_KEY: 'YOUR_API_KEY_HERE',  // Your Google API key
  SPREADSHEET_ID: 'YOUR_SPREADSHEET_ID_HERE',   // Your Sheet ID
  SHEET_RANGE: 'Sheet1!A1:O1000',
  ACCESS_PIN: '1234'  // CHANGE THIS PIN!
};
```

## 📊 Google Sheets Setup

1. Import `ama-selections-data.csv` to Google Sheets
2. Get your API key from Google Cloud Console
3. Make sheet public (Anyone with link can view)
4. Update the CONFIG above with your credentials

---

**Ready to deploy!** 🎉
