# 📘 Thesis Documentation Template (Markdown + MkDocs)

Welcome to the **Thesis Documentation Template** — a modern, modular, and GitHub-friendly way to write your thesis using:

- **Markdown** for clean writing  
- **MkDocs + Material theme** for beautiful documentation  
- **GitHub + GitHub Pages** for tracking progress and publishing  
- **GitHub Actions** for validating and deploying automatically  

This template follows a **standard academic thesis format** and breaks every section into separate Markdown files for clarity and maintainability.

---

# 📦 How to Use This Repository as a Template

This repository is configured as a **Template Repository** on GitHub.

If you are a student starting your thesis project, **DO NOT fork this repo**.  
Instead, follow these steps:

### ✅ 1. Click the **“Use this template”** button at the top of the repository

This will create a **brand‑new repository under your GitHub account** with the same content.

### ✅ 2. Name your repository

Example names:

- `thesis-juan-dela-cruz`
- `thesis-mary-anne`
- `capstone-group5`

Choose **Public** or **Private** depending on class requirements.

### ✅ 3. Clone your newly created repository

```bash
git clone https://github.com/<your-username>/<your-repo>.git
```

### ✅ 4. Start editing your Markdown files inside the `docs/` folder

When finished editing:

```bash
git add .
git commit -m "Add Chapter 1 Introduction"
git push
```

---

# 🧭 Notes for Students Who Already Forked Before This Template Was Enabled

If you already forked the teacher’s repo earlier:

### ✔ Your fork still works — you do NOT need to start over.

To receive updates from the teacher template:

```bash
git remote add upstream https://github.com/Kinev10/thesis-markdown-template.git
git pull upstream main
```

If your fork is broken or outdated, you may choose to:
- create a NEW repo using the template  
- copy your existing work into the new structure

---

# 📁 Repository Structure

Your thesis content lives entirely inside the `docs/` directory:

```
docs/
│
├── index.md
│
├── 01-front-matter/
│   ├── title-page.md
│   ├── abstract.md
│   ├── table-of-contents.md
│   ├── list-of-figures.md
│   ├── list-of-tables.md
│   └── list-of-notations.md
│
├── 02-introduction/
│   ├── project-context.md
│   ├── purpose-and-description.md
│   ├── objectives.md
│   └── scope-and-limitations.md
│
├── 03-related-literature/
│   └── related-literature.md
│
├── 04-technical-background/
│   └── technical-background.md
│
├── 05-design-and-methodology/
│   ├── conceptual-design.md
│   ├── system-architecture.md
│   ├── block-diagrams.md
│   └── algorithms.md
│
├── 06-results-and-discussion/
│   └── results-and-discussion.md
│
├── 07-conclusions-and-recommendations/
│   └── conclusions-and-recommendations.md
│
├── 08-appendices/
│   ├── source-code.md
│   ├── evaluation-tools.md
│   ├── sample-input-output.md
│   ├── user-guide.md
│   └── cv/
│       ├── member1.md
│       └── member2.md
│
├── img/
└── src/
```

This structure ensures your thesis is:

✔ Modular  
✔ Easy to manage  
✔ Easy to review  
✔ Ready for publication  

---

# 🧩 Requirements

Install MkDocs and the Material theme:

```bash
pip install mkdocs mkdocs-material
```

---

# ▶️ Local Preview

To preview your thesis website locally:

```bash
mkdocs serve
```

Open:

```
http://127.0.0.1:8000/
```

---

# 🌐 GitHub Pages Deployment

This project is designed to be published online using **GitHub Pages** and **MkDocs**.

---

## ✅ 1. Push your repository to GitHub

If you haven’t yet:

```bash
git add .
git commit -m "Initial commit"
git push
```

---

## ✅ 2. Automatic Deployment

This template includes a **GitHub Actions workflow** that automatically deploys your MkDocs site **whenever a Pull Request is merged into the `main` branch**.

The workflow will:

1. Build your MkDocs site  
2. Push the output to the `gh-pages` branch  
3. Update your GitHub Pages website  

---

## ✅ 3. One-Time Setup on GitHub Pages

After your first merge to main:

1. Go to **Settings**
2. Select **Pages**
3. Under *Build & Deployment*:
   - **Source:** Deploy from a branch
   - **Branch:** `gh-pages`
   - **Folder:** `/ (root)`
4. Save

Your thesis will be published at:

```
https://<username>.github.io/<repository-name>/
```

Example:

```
https://kinev10.github.io/thesis-markdown-template/
```

---

# 🔄 Updating Your Repository When the Template Is Updated

If your repo was created using the template, you can still sync improvements manually:

### Add upstream (ONE TIME ONLY)

```bash
git remote add upstream https://github.com/Kinev10/thesis-markdown-template.git
```

### Pull updates anytime

```bash
git pull upstream main
```

---

# 🤝 Contribution Guidelines (For Students)

Follow this workflow for clean collaboration:

---

## 1️⃣ Create a Feature Branch

```bash
git checkout -b feature/<your-topic>
```

Examples:

- `feature/add-abstract`
- `feature/update-methodology`
- `fix/typo-chapter3`

---

## 2️⃣ Write Clear Commit Messages

```
feat: add system architecture diagrams
fix: correct grammar in introduction
docs: update abstract formatting
```

---

## 3️⃣ Keep Pull Requests Small  
Do not mix unrelated edits.

---

## 4️⃣ Open a Pull Request

1. Push your branch  
2. Click **Compare & Pull Request**  
3. Describe your changes  
4. Submit  

---

## 5️⃣ Sync Before Working Again

```bash
git pull upstream main
```

---

# 🔄 Student Workflow Diagram

```mermaid
flowchart TD
    A[Fork or Use Template] --> B[Clone Repository]
    B --> C[Create Feature Branch]
    C --> D[Edit Thesis Pages in docs/]
    D --> E[Commit and Push Changes]
    E --> F[Open Pull Request to Main Repo]
    F --> G{Teacher Reviews PR}
    G -->|Approved| H[PR is Merged]
    H --> I[GitHub Actions Builds MkDocs Site]
    I --> J[GitHub Pages Updates Automatically]
    H --> K[Student Syncs with Upstream if Needed]
    K --> C
```

---

# ✍️ Editing Your Thesis

Modify content inside:

```
docs/
```

Images go inside:

```
docs/img/
```

Source code, scripts, datasets go inside:

```
docs/src/
```

---

# 🎉 You're Ready!

You now have a complete **Thesis Documentation Template** with:

✔ Clean academic structure  
✔ Markdown-based writing  
✔ Auto-validation on PRs  
✔ Auto-deployment to GitHub Pages  
✔ Template-based student workflow  
✔ Optional upstream sync  
✔ Visual contribution diagram  
