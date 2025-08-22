# Basic CI/CD Implementation with Simple Project

## 📖 Simple Story

Imagine you are building your **personal portfolio website**.  
Every time you make a small change (update a project, fix a typo, add a new skill), you have to:

1. Edit the code  
2. Build locally  
3. Unpublish the old site  
4. Publish the new version  

⏳ This cycle wastes time.  
🚨 Manual steps introduce mistakes.  
⚡ Productivity drops.

---

## 💡 Solution → CI/CD

With **Continuous Integration (CI)** and **Continuous Deployment (CD)**, the process becomes **automatic**:

- Push your code to **GitHub**  
- **GitHub Actions** runs:
  - ✅ Build  
  - ✅ Test  
  - ✅ Deploy  
- Your site updates automatically → no manual republish.

---

## 🔧 Tech Stack (Example)

- **GitHub Actions** → CI/CD pipeline  
- **Node.js / React** → Sample web project  
- **Docker** → Containerized build  
- **GitHub Pages / Vercel / Netlify** → Deployment target  

---

## 🚀 Workflow Example (GitHub Actions)

```yaml
name: CI/CD Pipeline

on:
  push:
    branches: [ "main" ]

jobs:
  build-deploy:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout Repository
        uses: actions/checkout@v3

      - name: Setup Node.js
        uses: actions/setup-node@v3
        with:
          node-version: 18

      - name: Install Dependencies
        run: npm install

      - name: Build Project
        run: npm run build

      - name: Deploy to GitHub Pages
        uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./build
