# Getting your JobTailor keys — step by step

You'll set up up to three keys. **Do them in this order.** The first two are free; Claude is optional (paid, best quality).

After you copy each key, open **JobTailor.html**, open the **⚙️ "Set up once"** panel at the top, paste the key into the matching box, and click **Save on this computer**.

A key is like a password — keep it private, and don't share your screen while it's visible.

---

## Key 1 — Google Gemini (free AI) — about 3 minutes

This powers the "understands your whole resume" writing, for free.

1. Go to **https://aistudio.google.com/app/apikey**
2. Sign in with any **Google account**.
3. If asked, accept the terms.
4. Click **Create API key**.
5. If it asks for a project, choose **Create API key in new project**.
6. Your key appears — it starts with **`AIza`**. Click the **copy** icon.
7. In JobTailor's ⚙️ panel, paste it into the **Google Gemini API key** box → **Save on this computer**.

**Good to know:** No credit card needed. Free limits are roughly 10 requests/minute and 500/day — plenty for personal use. If Google asks you to "restrict" the key, restrict it to the **Generative Language API** (leave application restrictions as None so it works from your computer).

---

## Key 2 — RapidAPI / JSearch (free — the big job sites) — about 3 minutes

This unlocks Indeed, LinkedIn, ZipRecruiter, and Glassdoor listings.

1. Go to **https://rapidapi.com/letscrape-6bRBa3QguO5/api/jsearch**
2. Click **Sign Up** (top right) and create a free account (Google/GitHub/email all work). **No credit card required.**
3. You'll land back on the **JSearch** API page. Click the **Pricing** tab.
4. On the **Basic** plan (the free one — about 200 searches per month), click **Subscribe**.
5. Go to the **Endpoints** tab. On the right side you'll see a code example. Find the line that says **`X-RapidAPI-Key`** and copy the long value next to it (just the key, not the quotes).
6. In JobTailor's ⚙️ panel, paste it into the **RapidAPI key** box → **Save on this computer**.

**Good to know:** Each "Find jobs" click uses 1 of your ~200 free monthly searches. If you run out, the free sources (Jobicy, The Muse) still work, or paste a job manually.

---

## Key 3 — Anthropic / Claude (optional — best quality, paid) — about 5 minutes

Only do this if you want Claude's writing. It is **billed per use** (usually pennies per job) and is **separate from your Claude.ai subscription**. New accounts usually get **$5 in free credit** after phone verification, which is enough to try it.

1. Go to **https://console.anthropic.com**
2. Sign up / sign in (this is the *developer console*, different from the Claude chat app).
3. Complete **phone verification** if prompted — this typically adds **$5 free credit** to your account.
4. Open **Settings → Billing** (also called "Plans & Billing"). To keep using it beyond the free credit, click **Add to credit balance** and add a small amount (e.g. **$5**). *This step matters — without any credit/billing, a brand-new key returns errors.*
5. Open **Settings → API keys**.
6. Click **Create Key**, give it a name like "JobTailor", and click create.
7. **Copy the key now** — it starts with **`sk-ant-`** and is shown only once.
8. In JobTailor's ⚙️ panel, paste it into the **Claude (Anthropic) API key** box.
9. In the **Use** dropdown choose **Auto** (or **Claude only**), and in **Claude quality** pick **Haiku 4.5** (cheapest) to start. → **Save on this computer**.

**Cost feel:** With Haiku, a job search + a tailored resume + cover letter is typically a fraction of a cent to a few cents. You can watch your usage in the Console under **Usage**.

---

## After you have your keys

1. In the ⚙️ panel, set **Use** to **Auto** (uses Claude if you added it, otherwise Gemini).
2. Click **Save on this computer** (you only do this once per computer).
3. Add your resume in Step 1, then click **Find jobs** in Step 2.

## If something doesn't work

- **Claude says "credit" or "billing" error** → add a small credit balance (Key 3, step 4).
- **A job search returns nothing** → a network or ad-blocker may be blocking the sites, or your RapidAPI free searches ran out. Use **"Or paste a specific job"** — paste a posting from Indeed/LinkedIn and it tailors perfectly.
- **You lost your Anthropic key** → you can't view it again; just create a new one and delete the old.
- **Sharing with friends** → each person needs their own keys. For friends, the free **Gemini** key is the easy choice (no cost).
