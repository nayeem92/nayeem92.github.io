# Football Analytics Site — Setup & How to Add New Reports

## One-time setup (GitHub Pages, free)

1. Go to github.com, click "New repository"
2. Name it **exactly** `nayeem92.github.io` (this exact name makes GitHub auto-host it at that URL)
3. Set it to Public, click "Create repository"
4. On the new repo page, click "uploading an existing file"
5. Drag in `index.html` and the whole `reports/` folder from this download
6. Commit the files
7. Wait ~1 minute — your site is live at **https://nayeem92.github.io**

No command line needed for this part.

## Adding a new report later

Each time you publish a new Kaggle notebook and want a report page for it:

1. Upload the `.ipynb` file to a chat with Claude
2. Ask for "the same report format" for it
3. Claude builds a new HTML file in the same visual style, pulling the real
   charts and findings straight from the notebook
4. Add that file into `reports/` in the GitHub repo (same drag-and-drop upload)
5. Add one new `<a class="card">` block to `index.html` linking to it — copy
   one of the existing card blocks and swap the title/description/link

That's the whole workflow — the template and styling stay consistent every time.
