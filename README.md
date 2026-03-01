# hetvaghela.com — Personal Portfolio

A clean, dark-themed personal portfolio site for Het Vaghela.

## 🛠 Customize Before Deploying

Open `index.html` and update every section marked with `<!-- UPDATE: -->`:

1. **Hero** — Your tagline/one-liner
2. **About** — Your bio paragraph
3. **Stats** — Years of experience, number of projects, etc.
4. **Skills** — Your actual tech stack
5. **Experience** — Your real job history and education
6. **Projects** — Your actual projects with real links & tags
7. **Contact** — Your real email and GitHub URL

---

## 🚀 Deploying to GitHub Pages (Free Hosting)

### Step 1 — Create a GitHub repository

1. Go to [github.com](https://github.com) and sign in (or create an account)
2. Click **New Repository**
3. Name it exactly: `hetvaghela.com` (or any name you want)
4. Set it to **Public**
5. Click **Create repository**

### Step 2 — Push this site

```bash
cd hetvaghela/
git init
git add .
git commit -m "Initial portfolio site"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/hetvaghela.com.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages

1. Go to your repo → **Settings** → **Pages**
2. Under **Source**, choose `main` branch and `/ (root)` folder
3. Click **Save**
4. GitHub will give you a URL like `https://yourusername.github.io/hetvaghela.com`

---

## 🌐 Pointing Your GoDaddy Domain to GitHub Pages

1. **Get GitHub Pages IP addresses** (current as of 2024):
   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```

2. **In GoDaddy DNS settings** (My Products → hetvaghela.com → DNS):
   - Delete any existing `A` records for `@`
   - Add 4 new `A` records, each pointing `@` to one of the IPs above
   - Add a `CNAME` record: Name = `www`, Value = `YOUR_USERNAME.github.io`

3. **In GitHub Pages settings**:
   - Under **Custom domain**, type `hetvaghela.com`
   - Check **Enforce HTTPS** (after DNS propagates ~24hrs)

4. Create a `CNAME` file in your repo root:
   ```
   hetvaghela.com
   ```

That's it! Within 24-48 hours, `hetvaghela.com` will serve your portfolio. ✅

---

## 🎨 Tech

- Pure HTML/CSS — no build tools, no dependencies
- Google Fonts (Syne + DM Sans)
- Fully responsive
