# Naila Ahmad Farooqi — Portfolio Website

A personal portfolio website for a Data Science & Analytics professional, built as a static site deployable on **GitHub Pages (free)**.

---

## 🚀 How to Deploy to GitHub Pages (Free)

### Step 1: Create a GitHub Account
Go to [github.com](https://github.com) and sign up (it's free).

### Step 2: Create a New Repository
1. Click the **+** button → **New repository**
2. Name it exactly: `your-username.github.io`  
   *(Replace `your-username` with your actual GitHub username)*
3. Set it to **Public**
4. Click **Create repository**

### Step 3: Upload Your Files
**Option A — Through the browser (easiest):**
1. Open your new repository
2. Click **uploading an existing file**
3. Drag and drop ALL the files from this folder
4. Make sure to keep the folder structure:
   ```
   index.html
   assets/
     css/style.css
     js/main.js
   projects/
     toronto-311.html
     toronto-homicide.html
     predictive-ml.html
     nlp-analysis.html
     health-analytics.html
   ```
5. Click **Commit changes**

**Option B — Using Git (recommended for ongoing updates):**
```bash
git init
git add .
git commit -m "Initial portfolio deploy"
git remote add origin https://github.com/your-username/your-username.github.io.git
git push -u origin main
```

### Step 4: Enable GitHub Pages
1. Go to your repository → **Settings** → **Pages**
2. Under **Source**, select `main` branch
3. Click **Save**
4. Your site will be live at: `https://your-username.github.io` in ~2 minutes!

---

## ✏️ How to Edit Content

### Update Your Info
All main content is in `index.html`. Search for sections marked with `<!-- ✏️ EDIT -->` comments.

### Add References
Find the `<!-- REFERENCES -->` section in `index.html` and replace the placeholder cards with real reference details.

### Add Recommendation Letters
Find the `<!-- RECOMMENDATIONS -->` section in `index.html`. You can:
- Link to a PDF: upload the PDF to a `assets/letters/` folder and update the button `onclick`
- Or paste the letter text into a new HTML page

### Add a New Project
1. Copy any file from the `projects/` folder
2. Rename it (e.g., `projects/my-new-project.html`)
3. Edit the content inside
4. Add a new card in `index.html` under the Projects section:
```html
<a href="projects/my-new-project.html" class="project-card">
  <div class="project-icon">📊</div>
  <div class="project-info">
    <h3>My New Project</h3>
    <p>Short description of the project.</p>
    <div class="project-tags"><span>Python</span><span>ML</span></div>
  </div>
  <div class="project-arrow">→</div>
</a>
```

### Add Notebook Visualizations
In each project page, find the `placeholder-viz` blocks and replace them with:
```html
<img src="../assets/images/your-chart.png" alt="Chart description" style="width:100%;border-radius:8px;" />
```
Upload your images to `assets/images/`.

---

## 📁 File Structure

```
portfolio/
├── index.html              ← Main portfolio page
├── README.md               ← This file
├── assets/
│   ├── css/
│   │   └── style.css       ← All styling
│   ├── js/
│   │   └── main.js         ← Navigation & animations
│   └── images/             ← Add your chart images here
└── projects/
    ├── toronto-311.html
    ├── toronto-homicide.html
    ├── predictive-ml.html
    ├── nlp-analysis.html
    └── health-analytics.html
```

---

## 💡 Tips
- **Custom domain:** Buy a domain (e.g., `nailafarooqi.com`) from Namecheap or Google Domains (~$10/year), then set it up under GitHub Pages settings.
- **Keep it updated:** Every time you push changes to GitHub, the site auto-updates within a minute.
- **LinkedIn link:** Update the LinkedIn URL in `index.html` to your actual profile URL.
