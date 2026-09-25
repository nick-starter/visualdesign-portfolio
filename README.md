# visualdesign-portfolio

Design portfolio — separate from `health-dashboard`. That repo is untouched.

## Local preview
Open `index.html` in a browser, or run `python3 -m http.server 8000` in this folder.

## Publish to GitHub Pages with custom URL
1. Create new repo on GitHub: `visualdesign-portfolio` (empty, no README)
2. Then run:
```
cd "/Users/nicholaschild/Documents/visualdesign-portfolio"
git init
git add .
git commit -m "Initial portfolio scaffold"
git branch -M main
git remote add origin git@github.com:nick-starter/visualdesign-portfolio.git
git push -u origin main
```
3. GitHub > repo Settings > Pages > Deploy from branch: `main` / `/ (root)`
4. Custom domain: Settings > Pages > Custom domain > enter `yourdomain.com` > Save.
5. DNS at registrar:
   - `A` @ to 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - `CNAME` www to nick-starter.github.io
6. Wait for DNS + check Enforce HTTPS.
