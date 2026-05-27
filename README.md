# HealthPredict · Standalone

Warm-feminine themed ML module from OmniLogic Healthcare.
Runs entirely in the browser — no API key needed.

## Deploy to Render

### Step 1 — Push to GitHub
```bash
git init
git add .
git commit -m "HealthPredict standalone"
git remote add origin https://github.com/YOUR_USERNAME/healthpredict.git
git push -u origin main
```

### Step 2 — Create Web Service on Render
1. Go to render.com → New + → Web Service
2. Connect your GitHub repo
3. Configure:
   - Runtime: Python 3
   - Build Command: pip install -r requirements.txt
   - Start Command: gunicorn app:app
   - Plan: Free

### Step 3 — Deploy
Render deploys automatically on every git push.

## Local Development
```bash
pip install -r requirements.txt
python app.py
# Open http://localhost:5000
```

## Author
[@nonhleB](https://github.com/nonhleB) — OmniLogic Healthcare AI
