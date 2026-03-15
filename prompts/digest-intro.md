# Digest Intro Prompt

You are assembling the final digest from individual source summaries.

## Format

Start with this header (replace [Date] with today's date):

AI Builders Digest — [Date]

Then organize content in this order:

1. PODCASTS section — list each podcast with new episodes
2. X / TWITTER section — list each builder with new posts

## AI Relevance Filter

Before including any content, check if it's related to AI, technology, or building products.
SKIP content that is clearly unrelated to AI/tech, such as:
- Personal life stories, relationships, or lifestyle content
- Generic business/career advice not tied to AI or tech
- Interviews focused on the person's personal journey rather than their AI/tech work
- Non-tech industry topics (unless AI is being applied to that industry)

When in doubt, include it — but if the episode or post has nothing to do with AI,
tech, or building products, leave it out entirely.

## Rules

- Only include sources that have new content AND pass the AI relevance filter
- Skip any source with nothing new or nothing AI-relevant
- Under each source, paste the individual summary you generated

### Podcast links
- After each podcast summary, include the specific video URL from the JSON `url` field
  (e.g. https://youtube.com/watch?v=Iu4gEnZFQz8)
- NEVER link to the channel page. Always link to the specific video.
- Include the exact episode title from the JSON `title` field in the heading

### Tweet author formatting
- Use the author's full name and role/company, not just their last name
  (e.g. "Box CEO Aaron Levie" not "Levie")
- NEVER write Twitter handles with @ in the digest. On Telegram, @handle becomes
  a clickable link to a Telegram user, which is wrong. Instead write handles
  without @ (e.g. "Aaron Levie (levie on X)" or just use their full name)
- Include the direct link to each tweet from the JSON `url` field

### General
- At the very end, add a line: "Reply to adjust your settings, sources, or summary style."
- Keep formatting clean and scannable — this will be read on a phone screen
