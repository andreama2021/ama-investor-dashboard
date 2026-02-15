# 📊 Investor Dashboard

A professional, real-time investor dashboard that pulls data from Google Sheets with PIN authentication and period-based analytics.

![Dashboard Preview](https://img.shields.io/badge/Status-Production%20Ready-success)
![React](https://img.shields.io/badge/React-18.2-blue)
![License](https://img.shields.io/badge/License-MIT-green)

## ✨ Features

- 🔐 **PIN Authentication** - Simple, secure access control
- 📈 **Real-time Data** - Automatically syncs with Google Sheets
- 📊 **Interactive Charts** - Beautiful visualizations with Recharts
- ⏰ **Period Filtering** - View data by 30 days, quarter, 6 months, year, or custom range
- 📉 **Growth Metrics** - Automatic period-over-period comparisons
- 📱 **Responsive Design** - Works perfectly on desktop, tablet, and mobile
- 🎨 **Professional UI** - Clean, modern interface that impresses investors

## 🎯 Key Metrics Tracked

### Financial Performance
- **Total GMV** - Gross Merchandise Value (Rentals + Services)
- **Total Revenue** - Revenue from rentals and services
- **TTM Revenue** - Trailing 12-month revenue
- **Average Booking Value** - Average villa rental value

### Operations
- **Total Bookings** - Villa rental count
- **Nights Booked** - Total nights across all bookings
- **Total Users** - Platform users
- **NPS Score** - Net Promoter Score

### Marketing & Runway
- **Marketing Spend** - Monthly marketing investment
- **Marketing Efficiency** - Revenue/Marketing ratio
- **Cash Position** - Current cash in bank
- **Runway** - Months of operation remaining

## 🚀 Quick Start

1. **Set up Google Sheets** (see sample-data.csv for template)
2. **Get Google Sheets API key** (instructions in SETUP-GUIDE.md)
3. **Configure** the dashboard (update CONFIG in src/investor-dashboard.jsx)
4. **Deploy** to Vercel/Netlify (5 minutes)

See [QUICK-START.md](QUICK-START.md) for step-by-step instructions.

## 📁 Project Structure

```
investor-dashboard/
├── src/
│   ├── main.jsx                 # React entry point
│   └── investor-dashboard.jsx   # Main dashboard component
├── index.html                   # HTML template
├── package.json                 # Dependencies
├── vite.config.js              # Build configuration
├── sample-data.csv             # Google Sheets template
├── SETUP-GUIDE.md              # Comprehensive setup guide
├── QUICK-START.md              # 5-minute deployment guide
└── README.md                   # This file
```

## 🛠️ Technology Stack

- **React 18** - UI framework
- **Recharts** - Data visualization
- **Tailwind CSS** - Styling
- **Vite** - Build tool
- **Google Sheets API** - Data source
- **Lucide React** - Icons

## 📊 Google Sheets Setup

Your sheet should have these 15 columns:

| Column | Description |
|--------|-------------|
| Date | YYYY-MM-DD format |
| GMV_Total | Total Gross Merchandise Value |
| GMV_Rentals | GMV from villa rentals |
| GMV_Services | GMV from additional services |
| Revenue_Total | Total revenue |
| Revenue_Rentals | Revenue from rentals |
| Revenue_Services | Revenue from services |
| Bookings | Number of bookings/rentals |
| Nights | Total nights booked |
| Avg_Booking_Value | Average value per booking |
| Users | Total platform users |
| NPS | Net Promoter Score |
| Marketing_Spend | Monthly marketing spend |
| Cash_Position | Current cash in bank |
| TTM_Revenue | Trailing 12-month revenue |

Use the `ama-selections-data.csv` file as a template - just import it to Google Sheets!

## 🔒 Security

- PIN-based authentication
- Session persistence
- API key can be restricted to Google Sheets API only
- Support for environment variables in production
- No sensitive data stored client-side

## 📱 Screenshots

### Login Screen
Clean, professional authentication with PIN entry.

### Main Dashboard
- 6 KPI cards with growth indicators
- 4 interactive charts (GMV, Bookings, Cash, Burn Rate)
- Period filtering controls
- Period-over-period comparison

## 🌐 Deployment Options

- **Vercel** (Recommended) - Zero-config, automatic HTTPS
- **Netlify** - Drag & drop deployment
- **GitHub Pages** - Free static hosting
- **Any static host** - It's just HTML/CSS/JS!

## 🔄 Updating Data

1. Update your Google Sheet
2. Dashboard automatically fetches latest data
3. Metrics recalculate in real-time

No manual uploads or complicated processes!

## 📈 Customization

The dashboard is fully customizable:

- Add more KPIs in the metrics section
- Change colors and branding
- Modify chart types
- Add new period filters
- Customize calculations

All well-commented code for easy modifications.

## 🐛 Support

Check the troubleshooting section in SETUP-GUIDE.md for common issues.

## 📄 License

MIT License - Use freely for personal or commercial projects.

## 🙏 Credits

Built with ❤️ for modern startups that need professional investor reporting.

---

**Ready to impress your investors?** Follow the QUICK-START.md guide and deploy in 5 minutes! 🚀
