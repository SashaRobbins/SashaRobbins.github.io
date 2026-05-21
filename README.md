# Portfolio Site — GitHub Pages

A clean, minimal portfolio site ready to upload to GitHub Pages.

---

## File Structure

```
your-repo/
├── index.html              ← Work / Projects page  (homepage)
├── about.html              ← About / Bio page
├── blog.html               ← Blog listing page
├── style.css               ← All styles (edit colours/fonts here)
├── images/                 ← PUT ALL YOUR IMAGES IN HERE
│   ├── project1.jpg
│   ├── me.jpg
│   └── ...
└── posts/                  ← Each blog post is its own HTML file
    ├── blog-post-template.html   ← Copy this to make a new post
    ├── post-title-one.html
    └── ...
```

---

## Quick Start (5 steps)

### 1. Upload all files to your GitHub repo
Drag and drop the files directly on GitHub.com into your Pages repo.
Your homepage must be named `index.html`.

### 2. Find every "CHANGE:" comment
Each file has `CHANGE:` comments in the code — these are the spots you need to edit.
Open the file in any text editor (Notepad, TextEdit, VS Code) and search for `CHANGE:`.

### 3. Replace placeholder text with your own
- Your name (appears in every nav bar and the footer)
- Page titles and descriptions (inside `<title>` tags)
- Bio paragraphs on about.html
- Project titles, descriptions, and tags on index.html

### 4. Add your images
1. Create an `images/` folder in your repo
2. Upload your image files there
3. In each HTML file, find the commented-out `<img>` tag and uncomment it:
   Change: `<!-- <img src="images/project1.jpg" alt="Project One" /> -->`
   To:     `<img src="images/project1.jpg" alt="Project One" />`
4. Delete the `<div class="placeholder">` line above it

### 5. Add blog posts
1. Copy `posts/blog-post-template.html`
2. Rename it to match your post, e.g. `posts/my-first-post.html`
3. Fill in the title, date, and content
4. Add a matching entry on `blog.html` pointing to it

---

## Changing Colours

Open `style.css` and find the `:root` block near the top:

```css
:root {
  --bg:           #FAF8F4;   /* page background    */
  --ink:          #1C1C1A;   /* main text colour   */
  --accent:       #B85C38;   /* links & highlights */
  ...
}
```

Change the hex colour values to your preferred colours.
Every colour on the site will update automatically.

---

## Changing the Font

In `style.css`, find this line near the top:

```css
@import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond...');
```

You can replace the font names with any Google Font.
Browse options at: https://fonts.google.com

---

## Adding / Removing Nav Links

If you want to add or remove pages, edit the `<ul class="nav-links">` block
in the `<nav>` section at the top of **each** HTML file.

---

## GitHub Pages Settings

1. Go to your repo → **Settings** → **Pages**
2. Under "Source", select **Deploy from a branch**
3. Choose `main` branch and `/ (root)` folder
4. Click Save — your site will be live at `https://yourusername.github.io/repo-name/`

---

## Need Help?

- GitHub Pages docs: https://docs.github.com/en/pages
- Google Fonts: https://fonts.google.com
- HTML colour picker: https://htmlcolorcodes.com
