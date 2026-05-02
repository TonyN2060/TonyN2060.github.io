# Tony Ndungu Munene — Portfolio

Personal portfolio site. Live at [tonymunene.com](https://tonymunene.com) (or `yourusername.github.io` if no custom domain).

## Deploy to GitHub Pages

### 1. Create the repo

Go to [github.com/new](https://github.com/new) and create a repo named **`yourusername.github.io`** (replace `yourusername` with your actual GitHub username). Leave it empty — don't add a README or .gitignore.

### 2. Push this folder

```bash
cd portfolio
git init
git add .
git commit -m "initial portfolio deploy"
git remote add origin https://github.com/YOUR_USERNAME/YOUR_USERNAME.github.io.git
git branch -M main
git push -u origin main
```

### 3. Enable GitHub Pages

- Go to your repo → **Settings** → **Pages**
- Source: **Deploy from a branch**
- Branch: **main** / root
- Click **Save**

Your site will be live at `https://yourusername.github.io` within 1-2 minutes.

### 4. Custom domain (optional)

If you've bought a domain (e.g. `tonymunene.com`):

1. Edit the `CNAME` file in this repo to contain your domain
2. In your domain registrar's DNS settings, add these **A records**:

   ```
   A  @  185.199.108.153
   A  @  185.199.109.153
   A  @  185.199.110.153
   A  @  185.199.111.153
   ```

3. Add a **CNAME record**:

   ```
   CNAME  www  yourusername.github.io
   ```

4. In GitHub repo → Settings → Pages → Custom domain, enter your domain
5. Check **Enforce HTTPS**

DNS propagation takes 5-30 minutes. After that your site is live on your domain with free HTTPS.

### 5. Update the site

Edit `index.html`, commit, and push:

```bash
git add .
git commit -m "update portfolio"
git push
```

Changes go live within a minute.

## Structure

```
portfolio/
├── index.html   ← the entire site (single file)
├── CNAME        ← custom domain config
└── README.md    ← this file
```

## Before you go live

Replace these placeholders in `index.html`:

- `href="#"` on LinkedIn → your actual LinkedIn URL
- `href="#"` on GitHub → your actual GitHub URL
- `href="#"` on Email → `mailto:your@email.com`
- `href="#"` on Scholar → your Google Scholar URL
- Update `CNAME` file with your actual domain (or delete it if using `yourusername.github.io`)
