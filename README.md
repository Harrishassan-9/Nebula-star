# Personalized Nebula Generator

A beautiful, interactive web app that transforms names into animated cosmic constellations with lightning strikes and explosions.

## Features

- 🌟 **Dynamic Constellation Generation**: Each name creates a unique star pattern
- ⚡ **Lightning Strike Effect**: Dramatic 3-second lightning that shatters the constellation
- 🚀 **Interactive Controls**: Zoom, pan, and explore the nebula
- 🎨 **Unique Visuals**: Seeded randomness ensures consistent but unique experiences per name
- 📱 **Responsive Design**: Works on all devices

## Deployment on Vercel

### Option 1: Deploy via Vercel CLI (Recommended)

1. **Install Vercel CLI**:
   ```bash
   npm install -g vercel
   ```

2. **Deploy**:
   ```bash
   vercel
   ```

3. **Follow the prompts**:
   - Link to existing project or create new
   - Choose your team/account
   - Confirm deployment settings

### Option 2: Deploy via Vercel Dashboard

1. **Push to GitHub** (if not already done):
   ```bash
   git add .
   git commit -m "Ready for deployment"
   git push origin main
   ```

2. **Go to [vercel.com](https://vercel.com)** and sign in

3. **Click "New Project"**

4. **Import your GitHub repository**

5. **Deploy** - Vercel will automatically detect it's a static site

## Project Structure

```
├── static/
│   ├── index.html      # Main application
│   └── style.css       # Styling
├── vercel.json         # Vercel configuration
├── app.py              # Flask backend (not needed for static deployment)
└── requirements.txt    # Python dependencies (not needed for static deployment)
```

## How It Works

1. **User enters their name** in the form
2. **Name is hashed** to create a unique seed
3. **Constellation is generated** using the seed for consistent results
4. **Stars appear progressively** one by one
5. **Lightning strikes** the constellation after completion
6. **Constellation explodes** into particles and fades away

## Customization

- **Lightning Duration**: Modify `lightningDuration` in the JavaScript (currently 3000ms)
- **Colors**: Adjust `hueBase` and `hueAccent` ranges
- **Animation Speed**: Modify `revealSpeed` and `tempo` values

## After Deployment

You'll get a URL like: `https://your-app-name.vercel.app`

Share this link with anyone to let them create their own personalized nebula!

## Troubleshooting

- **If deployment fails**: Check that all files are in the `static/` folder
- **If styles don't load**: Ensure `style.css` is in the same folder as `index.html`
- **If constellation doesn't appear**: Check browser console for JavaScript errors

## Performance

- **Static deployment** ensures fast loading
- **Canvas-based rendering** provides smooth animations
- **Optimized particle systems** maintain 60fps performance

