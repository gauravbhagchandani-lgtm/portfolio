# Gaurav Bhagchandani — Placement Portfolio v3

A clean, responsive, high-performance static placement portfolio built with HTML5, CSS3, and JavaScript.

## 🚀 Quick Deploy to Vercel

1. Push this repository to GitHub.
2. Go to [Vercel](https://vercel.com) and click **Add New Project**.
3. Select this GitHub repository.
4. Framework Preset: **Other** (Root directory: `.`).
5. Click **Deploy**.

That's it! Vercel will automatically serve `index.html` as the homepage, and all downloadable documents will be accessible under `/docs/`.

---

## 📁 Project Structure

```
Portfolio Link/
├── index.html              # Main portfolio webpage (Vercel entry point)
├── Portfolio Link v3.html   # Standalone copy of index.html
├── vercel.json             # Vercel routing & download headers configuration
├── package.json            # Project manifest
├── public/
│   ├── docs/              # Project documents (.pdf, .docx, .xlsx, .pptx, .html)
│   └── images/            # Assets (profile photo, logos)
└── README.md
```

---

## ➕ How to Add New Content in the Future

### 1. Add a New Project
Open `index.html` (and sync to `Portfolio Link v3.html`), navigate to the `projects` JavaScript array near line 380, and add a new object:

```javascript
{
  title: "Your Project Title",
  line: "A one-line summary of what the project accomplished.",
  story: "Detailed story and learnings behind the project...",
  btn1: { label: "View Document", link: "docs/your-file-name.pdf" },
  btn2: { label: "View Model", link: "docs/your-excel-file.xlsx" }
}
```

### 2. Add New Documents
Place any new PDF, Word, Excel, PowerPoint, or HTML files inside the `public/docs/` directory.

> **Tip for links**: Make sure to use `docs/your-file-name.ext` as the link path. Files with `.pdf`, `.docx`, `.xlsx`, or `.pptx` extensions will download automatically when clicked.

### 3. Update Profile Image or Logos
Replace `public/images/gaurav.png` or add new images inside `public/images/`.
