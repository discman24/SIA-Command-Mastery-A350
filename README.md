# A350 Non-Normal Mastery ★★★★
## Command Training Edition — PWA

Offline-capable Progressive Web App for A350 non-normal scenario training. Built for SIA command promotion preparation.

### Features
- **100+ scenarios** across 13 flight phases (Pre-Flight → Parking)
- **8 categories**: Technical, Passenger, Cabin/Crew, Operational, Weather, Security, Medical, ATC/Comms
- **CBTA assessment**: 10 competencies, 5-point performance scale
- **Flight Simulation**: Random scenario generation with point scoring
- **12-week program**: Structured learning path calibrated for experienced pilots
- **Offline ready**: Service worker caches everything for use without internet
- **Mobile/Tablet**: Touch-optimized, installable as home screen app

### Procedures Reference
- SIA FCOM Rev 18A
- A350 FCTM Rev 12
- SIA SQNP/SQSP/SQI Rev 18
- SIA OM Rev 31
- CBTA Competency Markers

**More restrictive of SIA and Airbus procedures always applies.**

### Deploy to Vercel
```bash
npm i -g vercel
vercel --prod
```

### Local Development
```bash
npx serve public -l 3000
```

### Install as App
1. Open in mobile browser (Chrome/Safari)
2. Tap "Add to Home Screen"
3. App works offline after first load

### Architecture
- Single-file HTML with React 18 via CDN
- Babel standalone for JSX transform
- localStorage for progress persistence
- Service Worker for offline capability
- No build step required
