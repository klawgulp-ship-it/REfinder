# PropHunter 🏚️

Distressed & off-market property finder with skip trace integration and built-in CRM.

## Features

- **Zip Code Search** - Enter any zip code to find distressed properties
- **Interactive Map** - Leaflet-powered map with property markers
- **Deal Rating System** - A+, B, C ratings based on deal score algorithm
- **Skip Trace Data** - Owner contact info (name, phone, email, mailing address)
- **Favorites** - Save properties for later
- **CRM with Reminders** - Track follow-ups with date reminders
- **Filter by Type** - Foreclosure, Tax Lien, Vacant, Probate, Pre-foreclosure

## Deploy to Railway

### Option 1: One-Click Deploy
1. Push this code to a GitHub repository
2. Go to [railway.app](https://railway.app)
3. Click "New Project" → "Deploy from GitHub repo"
4. Select your repository
5. Railway will auto-detect Node.js and deploy

### Option 2: Railway CLI
```bash
# Install Railway CLI
npm install -g @railway/cli

# Login
railway login

# Initialize project
railway init

# Deploy
railway up
```

## Local Development

```bash
# Install dependencies
npm install

# Start server
npm start

# Open http://localhost:3000
```

## Project Structure

```
prophunter/
├── public/
│   └── index.html    # Full app (HTML, CSS, JS in one file)
├── server.js         # Express server
├── package.json      # Dependencies & scripts
└── README.md         # This file
```

## Tech Stack

- **Frontend**: Vanilla JS, CSS (no framework bloat)
- **Map**: Leaflet.js with CartoDB dark tiles
- **Backend**: Express.js (static file server)
- **Storage**: LocalStorage (favorites, CRM)

## Notes

- Property data is generated mock data for demo purposes
- To use real data, integrate with APIs like:
  - PropStream
  - BatchLeads
  - REISift
  - Skip Genie (skip trace)
  
## Customization

To add real property APIs, modify the `generateProperties()` function in `public/index.html` to fetch from your data source instead of generating mock data.

---

Built for real estate investors 🏠
