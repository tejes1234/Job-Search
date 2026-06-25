# JobTailor — How to use it

A free tool you open in your browser and run on your own computer. Upload your resume (**Word, PDF, or text**), find **USA** tech jobs (**remote or in your state**) from the big sites, and let **AI read your whole resume** to tailor a resume + cover letter for each. Nothing is uploaded to a server — your resume goes only to the AI engine you choose and the job-search API (for keywords).

## One-time setup (the "⚙️ Set up once" panel at the top)

You need **one job-site key** and **at least one AI key**. Keys are remembered on this computer.

**AI engine — pick one or both (this is what reads the whole resume):**

- **Claude (best quality)** — go to **console.anthropic.com → API keys**, create a key, paste it into the Claude box. This is billed per use (usually pennies per job) and is **separate from your Claude.ai subscription** — a subscription alone can't power an app like this.
- **Google Gemini (free)** — go to **aistudio.google.com → Get API key**, paste it into the Gemini box.
- The **Use** dropdown lets you choose Auto (Claude if available, else Gemini), Claude only, or Gemini only. For Claude you can pick **Haiku** (cheapest) or **Sonnet** (best).

**Big job sites — Indeed, LinkedIn, ZipRecruiter, Glassdoor:**

- Go to **rapidapi.com**, search **JSearch**, subscribe to the **Basic (Free)** plan, copy the **X-RapidAPI-Key**, paste it into the RapidAPI box.
- Without this key, JobTailor still searches free job sources (Jobicy, The Muse).

*(With no keys at all it still runs in a basic keyword mode, but AI is what makes it understand your whole resume.)*

## Use it in 4 steps

1. **Open** `JobTailor.html` (double-click → opens in your browser).
2. **Add your resume** — upload a `.docx`, `.pdf`, or `.txt`, or paste it. With AI on, it reads the whole resume and shows how it understood you.
3. **Find jobs** — optionally type a role/keywords (AI can infer them from your resume if you leave it blank). Leave **State** blank + **Include remote** checked for remote-US only, or add a **State** to also include jobs there. Click **Find jobs**. The AI ranks each job by genuine fit to your whole background and shows a one-line reason.
4. **Tailor & download** — click **Tailor →** on a job, review the four tabs, and click **Download (Word)**. Tip: open in Word/Google Docs and "Save as PDF" if needed.

## Good to know

- **USA only:** results are filtered to United States roles — remote-US or your chosen state. Non-US listings are removed.
- **Whole-resume matching:** with AI on, ranking is based on your real field, level, and experience — not just keyword overlap — so unrelated jobs drop down or out.
- **It never invents experience.** Every AI prompt instructs it to use only facts in your resume and flag gaps instead of fabricating.
- **Costs:** Gemini and the job-sites key are free (with monthly limits). Claude charges a few cents per job to your Anthropic API account — you only pay when you use Claude.
- **If a search returns nothing:** a network/ad-blocker may be blocking the sites, or a key is missing/over quota. Use **"Or paste a specific job"** — paste a posting from Indeed/LinkedIn and it tailors perfectly.
- **Privacy:** your resume is sent only to the AI provider you chose (Anthropic or Google) and never stored by JobTailor.

## Sharing with friends

You can still send them the single `JobTailor.html` file. Each person adds their own free keys (and their own Anthropic key if they want Claude). Note: Claude usage is billed to whoever's key is used, so for friends, the free **Gemini** option is the easy choice.

## Not included (by design)

It doesn't auto-run on a schedule and doesn't apply to jobs for you — you run it whenever you like and submit applications yourself.
