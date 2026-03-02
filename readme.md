# Voyage — AI Travel Planner

## Deploy to Vercel (Free)

### Step 1 — Install Vercel CLI
```bash
npm install -g vercel
```

### Step 2 — Deploy
```bash
cd voyage-vercel
vercel
```
Follow the prompts (login with GitHub/Google, accept defaults).

### Step 3 — Add your secret API key
In the Vercel dashboard:
1. Go to your project → **Settings** → **Environment Variables**
2. Add a new variable:
   - **Name:** `GROQ_API_KEY`
   - **Value:** `gsk_your_actual_groq_key_here`
   - **Environment:** Production ✅  Preview ✅  Development ✅
3. Click **Save**
4. Go to **Deployments** → click the 3 dots on latest → **Redeploy**

### Done! 🎉
Your app is now live at `https://your-project.vercel.app`
- ✅ API key is 100% hidden from users
- ✅ Free hosting
- ✅ Free AI via Groq

## Project Structure
```
voyage-vercel/
├── index.html        ← The frontend app
├── api/
│   └── chat.js       ← Serverless function (holds your secret key)
└── vercel.json       ← Vercel config
```
