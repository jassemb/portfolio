# SEC_OPS // PORTFOLIO

DevSecOps engineer portfolio with a cyber-terminal aesthetic. Static HTML/CSS/JS — deployable to GitHub Pages with no build step.

## Preview locally

```bash
# Python
python3 -m http.server 8080

# Or Node.js
npx serve .
```

Open [http://localhost:8080](http://localhost:8080)

## Deploy to GitHub Pages

### 1. Create a GitHub repository

```bash
git init
git add .
git commit -m "Add DevSecOps portfolio site"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/portfolio.git
git push -u origin main
```

### 2. Enable GitHub Pages

1. Open your repo on GitHub → **Settings** → **Pages**
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**
3. Choose branch **main** and folder **/ (root)**
4. Click **Save**

Your site will be live at `https://YOUR_USERNAME.github.io/portfolio/` (or your custom domain if configured).

## Customize

| What to change | Where |
|----------------|-------|
| Email / resume links | `index.html` — hero buttons |
| Experience & projects | `index.html` — section content |
| Colors & fonts | `styles.css` — `:root` variables |
| GitHub repo URLs | `index.html` — `VIEW_REPOSITORY` links |

## Structure

```
portfolio/
├── index.html      # Main page
├── styles.css      # Cyber-terminal design system
├── script.js       # Animations & mobile menu
├── DESIGN.md       # Design tokens reference
└── screen.png      # Original design mockup
```

## License

MIT — use freely for your own portfolio.
# portfolio
