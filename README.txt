
# Bengali + Arabic Hugo PaperMod Starter

## Features
- Beautiful Medium-like reading experience.
- Bengali (LTR) + Arabic (RTL) support with proper fonts.
- Fully responsive PaperMod theme.
- Easy .docx → .md conversion with Pandoc.

## How to Use
1. Install Hugo Extended: https://gohugo.io/getting-started/installing/
2. Extract this ZIP.
3. Open a terminal in the folder.
4. Run: hugo server -D
5. Visit: http://localhost:1313

## Deployment (Free)
1. Push this folder to a **GitHub** repository.
2. Go to https://netlify.com → New Site from Git → Link your repo → Build command: `hugo` → Publish dir: `public`
3. Click deploy.

## Adding a New Post
1. Convert your `.docx` to `.md`:
   ```bash
   pandoc myfile.docx -f docx -t markdown -o content/posts/new.md
   ```
2. Ensure Arabic text is wrapped like:
   ```html
   <p lang="ar" dir="rtl">النص العربي هنا</p>
   ```
3. Run `hugo server -D` to preview.
