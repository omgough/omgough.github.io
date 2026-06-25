# Portfolio site — setup & deployment guide

A clean, single-file portfolio (`index.html`) ready to host **free** on GitHub Pages.
No build step, no framework, no dependencies. Just edit the HTML and push.

---

## What's in the folder

- `index.html` — the whole site (HTML + CSS in one file)
- `resume.pdf` — **you add this**: your CV (name it exactly `resume.pdf`)
- `headshot.jpg` — **you add this**: a square professional photo (name it exactly `headshot.jpg`)

---

## Step 1 — Edit your content

Open `index.html` in any text editor. Every spot you need to change is marked with
`<!-- EDIT: ... -->`. Use Find (Ctrl/Cmd-F) for `EDIT` to jump between them.

What to fill in:
- **Name, tagline, intro** (top of file, the "HERO" section)
- **Links** — email, GitHub, LinkedIn, Google Scholar (delete any you don't use)
- **About** — short bio. For the O-1A, emphasize impact, leadership, recognition, awards.
- **Projects** — duplicate a `<div class="card">` block for each project. Lead with metrics.
- **Publications** — one `<li>` per paper/talk. Bold your own name; include venue, year, links.
- **Resume** — drop your PDF in the folder as `resume.pdf`.

Tip: open `index.html` by double-clicking it to preview in your browser as you edit.

---

## Step 2 — Put it on GitHub

1. Create a free account at https://github.com if you don't have one.
2. Click **New repository**. Name it `yourusername.github.io`
   (use your actual GitHub username — this exact name makes the URL clean).
   Set it to **Public**, then **Create repository**.
3. On the new repo page, click **uploading an existing file**.
4. Drag in `index.html`, `resume.pdf`, and `headshot.jpg`. Click **Commit changes**.

---

## Step 3 — Turn on GitHub Pages

1. In the repo, go to **Settings → Pages**.
2. Under **Build and deployment → Source**, choose **Deploy from a branch**.
3. Set branch to **main** and folder to **/ (root)**. Click **Save**.
4. Wait ~1 minute. Your site is live at:
   **https://yourusername.github.io**

To update later: edit the files and re-upload (or push). Pages redeploys automatically.

---

## Step 4 (optional) — Custom domain

A custom domain (e.g. `yourname.com`) looks more professional on a petition.

1. Buy a domain (~$12/yr) from Namecheap, Cloudflare, Porkbun, etc.
2. In your repo: **Settings → Pages → Custom domain**, enter your domain, **Save**.
3. At your domain registrar, add DNS records:
   - Four `A` records for the apex domain (`@`) pointing to:
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - One `CNAME` record for `www` pointing to `yourusername.github.io`
4. Back in GitHub Pages, tick **Enforce HTTPS** (may take an hour to become available).

DNS can take up to a few hours to propagate.

---

## Notes for the O-1A petition

This site supports several O-1A evidentiary criteria — original contributions of major
significance, authorship of scholarly articles, and your professional record. To make it
work hardest for you:

- **Be specific and quantified.** "Reduced latency 40%," "12k GitHub stars," "cited 80×"
  beats vague claims.
- **Link primary sources.** Real repos, real papers, real talk recordings. Reviewers and
  your immigration attorney can verify them.
- **Keep it current and consistent** with your resume and petition letters.

This is a supporting exhibit, not legal evidence on its own — coordinate the framing with
your immigration attorney.
