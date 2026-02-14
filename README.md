# mrvl-team.github.io
Repo hosting the official website for M+RVL (Mechanisms of Positive-Strand RNA Virus Laboratory).

# M+RVL Lab Website: Quarto Setup Tutorial

### **1. Prerequisites**
Ensure the following are installed locally:
* **R** & **RStudio**
* **Git**
* **Quarto CLI**
---
### **2. Git Configuration**
Open the RStudio Terminal and configure your identity:

```bash
git config --global user.name "Your Username"
git config --global user.email "your.email@example.com"
```

---

### **3. Project Initialization**
1. **Create Project:** In RStudio, go to **File > New Project > Version Control > Git**.
2. **Clone:** Paste your existing GitHub repository URL and create the project.
3. **Initialize Quarto:** In the RStudio Terminal, run:
   ```bash
   quarto create project website .
   ```

---

### **4. Preview & Version Control**
**Preview Website:**
To view changes locally, run in Terminal:
```bash
quarto preview
```

**Commit & Push:**
When ready to save changes to the `main` branch:
```bash
git add .
git commit -m "Adding initial website files"
git push -u origin main
```

---

### **5. Deployment (GitHub Pages)**
**Render & Publish:**
Inside your website directory, run:
```bash
quarto publish gh-pages
```

**Verify Settings on GitHub:**
1. Go to your repository **Settings > Pages**.
2. Under **Build and deployment**:
   * **Source:** Deploy from a branch.
   * **Branch:** Select `gh-pages` and `/ (root)`.
3. Click **Save**.
