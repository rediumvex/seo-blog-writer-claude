# SEO Blog Writer — Claude Skill
![telegram-cloud-photo-size-4-5963180594780900429-y](https://github.com/user-attachments/assets/5d75ed29-b450-4d62-8b83-f962b56ca401)



> **SEO blog writer for Claude Code.** Turn any URL, notes, or topic into a
> human-sounding blog post that ranks on Google and beats AI detectors.
> Fills every SEO field, FAQ schema, and meta tag in one prompt.

**This is the actual Claude skill I use to write every post on [knoxhub.io](https://knoxhub.io).**
Not a template. Not a demo. The real thing — copied straight from my `~/.claude/skills/`.

---

## What it does

You give it anything — a URL, raw notes, a topic, a competitor's post, a YouTube transcript.
It gives you back a complete blog post with:

- **Human tone** — burstiness, perplexity, real slang, zero AI filler phrases
- **E-E-A-T signals** — first-person experience markers, specific numbers, real opinions
- **Full SEO fields** — title, meta description, focus keywords, alt text
- **FAQ schema** — ready for Google rich snippets
- **Table of contents** + sticky sidebar HTML
- **Internal link suggestions**
- **Markdown content** — drop it straight into your CMS

One prompt in, finished post out.

---

## Why human tone is the only SEO factor that still works in 2026

Google's helpful content update killed generic AI writing.
AI detectors (GPTZero, Originality.ai) flag 90% of raw ChatGPT output.
Both punish the same thing: **content that sounds like a robot wrote it.**

This skill enforces 6 anti-detection rules on every sentence:

1. **Burstiness** — mix 3-word sentences with 40-word ones
2. **Perplexity** — use real slang, unexpected word choices
3. **E-E-A-T** — add first-person experience every 500 words
4. **Zero filler** — ban "In today's world", "It's important to note", "delve into", etc.
5. **Sandwich method** — hand-write the hook and H2s
6. **Unpredictable format** — 4, 6, 7, or 9-item lists; never exactly 5

The result: content that ranks, doesn't trip detectors, and actually sounds like you wrote it.

---

## Install

```bash
# Clone into your Claude skills folder
cd ~/.claude/skills
git clone https://github.com/rediumvex/seo-blog-writer-claude.git seo-blog-writer
```

Restart Claude Code. The skill is now available as `/seo-blog-writer` (or whatever you name the folder).

### If you use gstack

```bash
cd ~/.claude/skills/gstack
git clone https://github.com/rediumvex/seo-blog-writer-claude.git
```

---

## Usage

Just send Claude your material:

```
/seo-blog-writer https://some-article-you-want-to-rewrite.com
```

```
/seo-blog-writer write a post about n8n vs Zapier for solo founders
```

```
/seo-blog-writer here are my raw notes: [paste notes]
```

You get back every field filled, ready to copy-paste into your CMS:

- Post title (H1)
- Short description / excerpt
- Category + tags
- SEO title (max 60 chars)
- Meta description (max 160 chars)
- Focus keywords
- Cover image alt text
- FAQ schema (3–5 Q&As)
- Table of contents
- Sticky sidebar HTML widget
- Full article content in Markdown

---

## Fork for your blog

The skill is pre-configured for [knoxhub.io](https://knoxhub.io). To adapt it to your own blog, open `SKILL.md` and edit three sections:

1. **Voice & Tone** — change `Roman Knox` to your name and your positioning
2. **Content Pillars** — list your blog's topics instead of Knox Hub's
3. **Internal Links** — replace with your own post URLs, or delete the section

Five minutes of work. Everything else — the anti-AI rules, SEO field structure, FAQ schema generation — works out of the box for any blog.

---

## Who built this

I'm **Roman Knox**. I run [Knox Community](https://www.skool.com/knox-community-7232/) — a Skool community of builders shipping AI products that actually make money.

I built this skill because I was spending 4 hours per post manually hand-editing AI output to sound human. Now it's one prompt.

- 🎓 **[Join Knox Community on Skool](https://www.skool.com/knox-community-7232/)** — n8n library, cold outreach systems, and the full stack of Claude skills that power knoxhub.io
- 📸 Instagram — [@roman.knox](https://www.instagram.com/roman.knox) · 280K+ followers
- 📚 Knox Hub — [knoxhub.io](https://knoxhub.io) — see the skill in action on every post
- 🤖 My other Claude skills — [Social Media Caption Generator](https://github.com/rediumvex/social-media-caption-generator-claude), [AI Video Generator](https://github.com/rediumvex/ai-video-generator-claude)

---

## License

MIT — do whatever you want with it. If it helps, a ⭐ on the repo is appreciated.
