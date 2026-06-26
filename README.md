# JobTailor

**JobTailor** is a free tool that tailors your résumé and cover letter to specific **U.S. tech jobs**. It runs entirely in your web browser — your résumé and your API keys stay on your own computer and are never uploaded to anyone.

Give it your résumé and it will:

- Find relevant U.S. jobs (remote, or in a state you choose) from several job sources, including Indeed, LinkedIn, ZipRecruiter, and Glassdoor.
- Use AI to read your **whole résumé** and rank jobs by genuine fit (not just keywords).
- Generate a polished, **tailored résumé + cover letter** for any job (download as PDF or Word).
- Produce a **"How to apply"** sheet with **50 likely interview questions** specific to that job.

---

## Two ways to use it

- **Online (easiest):** open the hosted link, if the owner enabled GitHub Pages:
  `https://YOUR-USERNAME.github.io/jobtailor/`
  Nothing to download — it opens right in your browser.
- **On your computer:** download **`JobTailor.html`** and double-click it to open in your browser (Chrome, Edge, Safari, Firefox).

Either way, **you add your own free keys** (below). They are saved only in *your* browser.

---

## Add your own API keys (one time, about 5 minutes)

Open the **⚙️ "Set up once"** panel at the top of the app and add at least one AI key plus the job-sites key. Click **Save on this computer** when done.

### 1) Google Gemini — free AI (recommended to start)

1. Go to **https://aistudio.google.com/app/apikey**
2. Sign in with any Google account; accept the terms if asked.
3. Click **Create API key** (choose *Create API key in new project* if prompted).
4. Copy the key (it starts with `AIza`) and paste it into the **Gemini** box.
   *No credit card required.* If Google asks you to restrict the key, restrict it to the **Generative Language API**.

### 2) RapidAPI / JSearch — free, unlocks the big job sites

1. Go to **https://rapidapi.com/letscrape-6bRBa3QguO5/api/jsearch**
2. Click **Sign Up** and create a free account (no credit card).
3. Open the **Pricing** tab and **Subscribe** to the **Basic (Free)** plan (~200 searches/month).
4. Open the **Endpoints** tab; on the right, copy the **X-RapidAPI-Key** value.
5. Paste it into the **RapidAPI key** box.
   *This also powers the Monster results. Job search needs at least one job-site key — this one, or the Adzuna/USAJobs keys below.*

### 3) (Optional) Anthropic Claude — best quality, paid per use

1. Go to **https://console.anthropic.com** (the developer console, not the Claude chat app).
2. Sign in and complete phone verification (usually adds **$5 free credit**).
3. **Settings → Billing** → add a small credit balance to keep using it.
4. **Settings → API keys → Create Key**; copy the key (starts with `sk-ant-`, shown once).
5. Paste it into the **Claude** box, set **Use** to *Auto* or *Claude*, and pick **Haiku** (cheapest) to start.
   *Billed per use (usually a few cents per job) to your own Anthropic account — separate from a Claude.ai subscription.*

### 4) (Optional) More job sources — Adzuna & USAJobs (both free)

These add extra listings via the ⚙️ **"More job sources"** section. Note: both are built for servers, so a browser sometimes blocks them — if a source fails, the **"Why:"** line under your results shows the reason.

**Adzuna — all-industry US listings:**

1. Go to **https://developer.adzuna.com/signup** and register (free).
2. On your dashboard, copy your **Application ID** and **Application Key**.
3. Paste them into the **Adzuna App ID** and **Adzuna App Key** boxes.

**USAJobs — federal jobs:**

1. Go to **https://developer.usajobs.gov/apirequest/** and fill out the form with your email.
2. They email you an **Authorization Key** (your API key).
3. Paste the key into **USAJobs API key**, and put the **same email** you registered into the **USAJobs email** box (their API requires it).

> **For the fullest coverage**, connect the official **Indeed / ZipRecruiter / Dice** connectors inside Claude and search there — see *Bonus* at the bottom.

---

## How to use it

1. **Add your résumé** in Step 1 — upload `.docx`, `.pdf`, or `.txt`, or paste it. Your name, email, and phone are pulled in automatically.
2. **Find jobs** in Step 2 — optionally type a role/keywords, leave **State** blank + **Include remote** checked for remote-US only, or add a state. Click **Find jobs**.
3. **Tailor** — click *Tailor →* on a job. Review the **Tailored résumé**, **Cover letter**, **How to apply** (with 50 interview questions), and **Match & gaps** tabs.
4. **Download** — use the **PDF** or **Word** buttons. The preview matches the download exactly.

---

## Privacy & costs

- JobTailor runs **client-side** in your browser. Your résumé is sent only to the AI provider you choose (Google or Anthropic) and to the job-search API (your keywords only).
- **Your keys are stored only in your browser** (local storage). They are never part of the shared file and are never sent to the person who shared the app. Use the **Clear saved keys** button to remove them from a browser.
- **Free tiers:** Gemini and the RapidAPI/JSearch Basic plan are free with monthly limits. **Claude** is billed to your own Anthropic account.
- Always **review every generated document** before sending it to an employer.

---

## Disclaimer

This is a free, community tool. It is **not affiliated with or endorsed by** Anthropic, Google, RapidAPI, Indeed, LinkedIn, ZipRecruiter, Glassdoor, or any job board. You are responsible for your own API usage and any associated costs, for complying with each provider's and job site's terms, and for the accuracy of anything you submit. Provided "as is," without warranty.

## License

Free to use, modify, and share.
