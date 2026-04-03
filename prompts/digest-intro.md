# Digest Intro Prompt

You are assembling the final digest from individual source summaries.

## Format

Start with this header (replace [Date] with today's date):

AI Builders Digest — [Date]

Then organize content in this order:

1. OFFICIAL BLOGS section — list each blog post from AI company blogs (OpenAI, Anthropic, etc.)
2. X / TWITTER section — list each builder with new posts
3. PODCASTS section — list each podcast with new episodes

## Rules

- Only include sources that have new content
- Skip any source with nothing new
- Under each source, paste the individual summary you generated

### Podcast links
- After each podcast summary, include the specific video URL from the JSON `url` field
  (e.g. https://youtube.com/watch?v=Iu4gEnZFQz8)
- NEVER link to the channel page. Always link to the specific video.
- Include the exact episode title from the JSON `title` field in the heading

### Tweet author formatting
- **ABSOLUTE RULE: You MUST use a strict NUMBERED FORMAT for each builder.** 
- Start every single builder's section exactly with this pattern: "[N] [Author Full Name] ([Company/Role])" (e.g. "[1] Aaron Levie (Box CEO)", "[2] Amjad Masad (Replit CEO)").
- Do NOT add a custom title or headline before the author's name. The numbered author name MUST be the only heading for that section.
- You MUST continue numbering sequentially for every builder in the list: [1], [2], [3], [4], etc. 
- **DO NOT put ANY emojis at the start of the line.** Emojis break the numbering format.
- Use the author's full name and role/company, not just their last name
  (e.g. "Box CEO Aaron Levie" not "Levie")
- NEVER write Twitter handles with @ in the digest. On Telegram, @handle becomes
  a clickable link to a Telegram user, which is wrong. Instead write handles
  without @ (e.g. "Aaron Levie (levie on X)" or just use their full name)
- Include the direct link to each tweet from the JSON `url` field
- **Add a short separator line (---) AND an empty line before and after it between each builder's section to ensure clear visual separation.**

#### ONE-SHOT EXAMPLE (PERFECT FORMAT):
Here is exactly how a builder's section MUST look:

[1] Aaron Levie (BOX CEO)
Argues that the productivity gains brought by AI agents will ultimately be constrained by key factors like security, compliance, and governance. He points out that the idea of enterprises letting agents generate code on their own (vibe code) is somewhat unrealistic, because in an enterprise environment, people cannot take on the full risk of every technology. He emphasizes there is no free lunch in AI productivity, and companies must build robust systems and processes to control agents.
https://x.com/levie/status/2039216522028257549 [2026-04-01 01:41PM, 96 likes]


---

### Blog post formatting
- Use the blog name as a section header (e.g. "Anthropic Engineering", "OpenAI News", "Claude Blog")
- Under each blog, list each new post with its title and summary
- Include the author name if available
- Include the direct link to the original article

### Mandatory links
- Every single piece of content MUST have an original source link
- Blog posts: the direct article URL (e.g. https://www.anthropic.com/engineering/...)
- Podcasts: the YouTube video URL (e.g. https://youtube.com/watch?v=xxx)
- Tweets: the direct tweet URL (e.g. https://x.com/levie/status/xxx)
- If you don't have a link for something, do NOT include it in the digest.
  No link = not real = do not include.

### No fabrication
- Only include content that came from the feed JSON (blogs, podcasts, and tweets)
- NEVER make up quotes, opinions, or content you think someone might have said
- NEVER speculate about someone's silence or what they might be working on
- If you have nothing real for a builder, skip them entirely

### General
- **Style requirement: No emojis, concise and direct.** Do not use any emojis anywhere in the digest.
- At the very end, add a line: "Generated through the Follow Builders skill: https://github.com/laoshi1991/follow-ai-builders"
- Keep formatting clean and scannable — this will be read on a phone screen
