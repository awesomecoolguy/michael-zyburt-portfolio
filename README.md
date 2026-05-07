# Michael Zyburt Portfolio Website

Modern, responsive personal portfolio for Michael Zyburt (Dual Electrical & Aerospace Engineer, UC Irvine).

## Features
- Clean dark theme with cyan accents (#00d4ff)
- 13 detailed engineering projects with photos, descriptions, and "What I Learned & Did" sections
- Fully interactive AI chatbot assistant (client-side JavaScript)
- Smooth animations, mobile-first responsive design
- Self-contained single-file HTML (easy to host)

## Live Demo
After deploying to GitHub Pages, your site will be live at:  
`https://yourusername.github.io/michael-zyburt-portfolio`

## How to Deploy on GitHub (Step-by-Step)

### 1. Prepare Your Local Folder
- Create a new folder on your computer called `michael-zyburt-portfolio`
- Copy your **index.html** (the one with the chatbot added — see instructions below)
- Copy all your local image files into the same folder:
  - board1.jpg
  - usb.png
  - moonbounce1.jpg
  - avionics1.png
  - balloon1.jpg
  - rover1.png
  - levitation1.jpg
  - car1.png
  - plane1.jpg
  - alarm1.jpg
  - powerdevice1.jpg
  (Any other images you use)

### 2. Create GitHub Repository
1. Go to [github.com](https://github.com) and log in (create account if needed).
2. Click the **+** icon (top right) → **New repository**.
3. Repository name: `michael-zyburt-portfolio`
4. Description: `Personal portfolio website with AI chatbot`
5. Set to **Public**
6. **Do NOT** initialize with README (we'll push our own)
7. Click **Create repository**

### 3. Upload Files via GitHub Web Interface (Easiest for Beginners)
1. On the new repo page, click **uploading an existing file**.
2. Drag and drop your entire folder contents (index.html + all .jpg/.png images).
3. Add a commit message: "Initial portfolio with AI chatbot"
4. Click **Commit changes**

### 4. Enable GitHub Pages
1. Go to your repo → **Settings** tab (top right)
2. Scroll down to **Pages** section (left sidebar)
3. Under "Build and deployment":
   - Source: **Deploy from a branch**
   - Branch: **main** (or master)
   - Folder: **/ (root)**
4. Click **Save**
5. Wait 1-2 minutes — your site will be live!

### 5. Access Your Live Site
Your portfolio will be available at:  
`https://YOUR_GITHUB_USERNAME.github.io/michael-zyburt-portfolio`

(Replace YOUR_GITHUB_USERNAME with your actual GitHub username)

### 6. Custom Domain (Optional)
If you own a domain, you can add it in the same Pages settings.

## Customizing the Chatbot

The chatbot is 100% client-side JavaScript (no backend, no API keys, works on GitHub Pages).

### Location in Code
Open `index.html` and find the JavaScript section near the bottom.

### How to Add New Responses
Edit the `getBotResponse(query)` function:

```javascript
function getBotResponse(query) {
  const q = query.toLowerCase();
  
  if (q.includes('your new keyword')) {
    return "Your custom response here!";
  }
  
  // ... existing responses
}
```

**Tips:**
- Put specific questions first (e.g., "rocket project" before general "project")
- Use `q.includes('word1') || q.includes('word2')`
- Keep responses friendly and professional
- Test by opening the HTML locally in your browser

### Quick Reply Buttons (Optional Enhancement)
You can add clickable chips in the initial bot message for common questions like:
- "Tell me about your projects"
- "What is your education?"
- "Show me your skills"

## File Structure
```
michael-zyburt-portfolio/
├── index.html          ← Main website + chatbot
├── board1.jpg
├── usb.png
├── moonbounce1.jpg
├── avionics1.png
├── balloon1.jpg
├── rover1.png
├── levitation1.jpg
├── car1.png
├── plane1.jpg
├── alarm1.jpg
├── powerdevice1.jpg
└── README.md           ← This file
```

## Browser Compatibility
- Chrome, Firefox, Safari, Edge (latest versions)
- Fully responsive on mobile/tablet

## Need Help?
- Open an issue on GitHub
- Email: michaelzyburt@gmail.com

---

**Built with ❤️ by Michael Zyburt | 2026**

*This portfolio showcases real engineering work — from high-altitude balloons to autonomous rovers and beyond.*
