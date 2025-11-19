# EBM Website Setup Instructions

## Quick Start - Dynamic Chapter Loading

This website **automatically discovers and loads any number of chapters or appendices** from your GitHub repository. No code changes needed when you add new files!

### Step 1: Create a GitHub Repository
1. Go to [github.com](https://github.com) and sign in (or create an account)
2. Click the `+` icon → "New repository"
3. Name it something like `ebm-book`
4. Make it **Public** (so the website can access it)
5. Click "Create repository"

### Step 2: Upload Your Markdown Files
1. In your new repository, click "Add file" → "Upload files"
2. Upload your markdown files with these naming patterns:
   - **Chapters**: `Chapter_1.md`, `Chapter_2.md`, `Chapter_3.md`, etc.
   - **Appendices**: `Appendix_A.md`, `Appendix_B.md`, `Appendix_C.md`, etc.
   - Any filename matching `Chapter_*` or `Appendix_*` will be automatically discovered!
3. Click "Commit changes"

### Step 3: Configure the Website (One Time!)
1. Open `index.html` in a text editor
2. Find this section at the top of the `<script>` tag:
```javascript
const GITHUB_CONFIG = {
    owner: 'YOUR_GITHUB_USERNAME',      // Change this!
    repo: 'YOUR_REPO_NAME',             // Change this!
    branch: 'main',                     // Usually 'main' or 'master'
    folder: '',                         // Leave empty if files are in root
    filePattern: /^(Chapter|Appendix)_\d+.*\.md$/i
};
```

3. Replace only these two values:
   - `YOUR_GITHUB_USERNAME`: Your GitHub username
   - `YOUR_REPO_NAME`: Your repository name (e.g., `ebm-book`)

**Example:**
```javascript
const GITHUB_CONFIG = {
    owner: 'john-doe',
    repo: 'ebm-book',
    branch: 'main',
    folder: '',
    filePattern: /^(Chapter|Appendix)_\d+.*\.md$/i
};
```

### Step 4: Test It
1. Open `index.html` in your browser
2. The sidebar should automatically populate with all chapters and appendices
3. Click any chapter to load it!

---

## Adding New Chapters or Appendices

**No code changes needed!** Just:

1. Create a new markdown file following the naming pattern:
   - `Chapter_4.md`, `Chapter_5.md`, etc.
   - `Appendix_D.md`, `Appendix_E.md`, etc.
2. Upload to your GitHub repository
3. Reload the website
4. New chapters appear automatically in the sidebar and home page grid!

---

## Naming Convention

Files are automatically discovered if they match this pattern:
- Start with `Chapter` or `Appendix` (case-insensitive)
- Followed by `_` and a number or letter
- End with `.md`

**Valid examples:**
- `Chapter_1.md` ✅
- `Chapter_2.md` ✅
- `Appendix_A.md` ✅
- `Appendix_B.md` ✅
- `Chapter_10.md` ✅ (numbers sort numerically)
- `Appendix_1.md` ✅

**Invalid examples:**
- `Chapter1.md` ❌ (missing underscore)
- `chapter_1.md` ❌ (must start with capital C or A)
- `Introduction.md` ❌ (must start with Chapter or Appendix)

---

## Organization

Files are automatically organized:
- **Chapters** (Chapter_1, Chapter_2, etc.) appear first in the sidebar
- **Appendices** (Appendix_A, Appendix_B, etc.) appear below chapters
- Both are sorted numerically/alphabetically

---

## Deployment Options

### Option A: Host on GitHub Pages (Free)
1. In your GitHub repo, go to Settings → Pages
2. Under "Source", select "Deploy from a branch"
3. Choose `main` branch and `/root` folder
4. Click Save
5. Your site will be available at: `https://YOUR_USERNAME.github.io/ebm-book/`

### Option B: Host Anywhere Else
- Upload `index.html` to any web host (Netlify, Vercel, your own server, etc.)
- The site will work as long as it can reach GitHub

### Option C: Local File
- Just open `index.html` directly in your browser
- Works offline after initial load

---

## Features

✅ **Automatic discovery** - No code changes when adding chapters  
✅ **Dynamic navigation** - Sidebar auto-populates with all chapters/appendices  
✅ **Smart sorting** - Chapters first, then appendices; numbered numerically  
✅ **Beautiful grid** - Home page shows all sections with alternating colors  
✅ **Responsive design** - Works on desktop, tablet, and mobile  
✅ **Fast loading** - Uses GitHub's raw content API for quick delivery  
✅ **No dependencies** - Just HTML + JavaScript, no database needed  

---

## File Structure Example

```
your-repo/
├── Chapter_1.md
├── Chapter_2.md
├── Chapter_3.md
├── Chapter_4.md
├── Appendix_A.md
├── Appendix_B.md
└── README.md (optional)
```

Or with subfolders:
```
your-repo/
├── content/
│   ├── Chapter_1.md
│   ├── Chapter_2.md
│   ├── Appendix_A.md
│   └── ...
└── (set folder: 'content' in GITHUB_CONFIG)
```

---

## Troubleshooting

### No chapters showing up
- **Check repository is public**: Go to repo Settings → General → visibility should be "Public"
- **Verify GITHUB_CONFIG**: Make sure `owner` and `repo` match your GitHub username and repo name
- **Check filenames**: Must match pattern (Chapter_#.md or Appendix_X.md)
- **Open console**: Press F12, go to Console tab - error messages show what's wrong

### Files exist but don't appear
- Hard refresh your browser (Ctrl+F5 or Cmd+Shift+R)
- GitHub can take a moment to serve new files
- Check console for the exact error message

### "Configuration Required" error
- You haven't set the GITHUB_CONFIG correctly
- Open index.html in editor and update owner/repo values
- Both must match your actual GitHub username and repository name

### Want to use a private repo?
- You'll need to generate a GitHub Personal Access Token
- Instructions available on request - let me know if you need help!

---

## Browser Console

For debugging, open Developer Tools (F12 or Cmd+Option+I) and check the Console tab. You'll see:
- URLs being fetched
- Files discovered
- Any errors with details

---

## Need Help?

All questions should be answerable by checking:
1. Browser console (F12) for error messages
2. GitHub repo settings (must be public)
3. Filename pattern (Chapter_#.md or Appendix_X.md)
4. GITHUB_CONFIG values match your actual GitHub account

---

Enjoy your dynamic EBM website! 📚
