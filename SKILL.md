# SEO Blog Post Generator

**Version:** 1.0.0
**Author:** max_0x1
**Category:** Content Marketing
**License:** MIT-0

## What This Skill Does

Generates SEO-optimized blog content from a single brief. Four prompt templates cover every format you need: full long-form articles, structured outlines, listicles, and FAQ/People Also Ask content blocks ready for schema markup.

Stop paying $150-500 per article to freelancers. Stop letting content be the bottleneck in your SEO strategy.

## Who It's For

- Solopreneurs and small business owners who need consistent blog content
- Content marketers and SEO specialists running multiple client sites
- Agency owners producing content at scale
- Bloggers and affiliate marketers targeting long-tail keywords
- SaaS founders building organic traffic before paid acquisition

## Prompt Templates

### 1. Full Long-Form Article (`prompts/full-article.md`)
Generates a complete 1,500-2,000 word article with:
- SEO title (55-60 chars) + alt H1 option
- Meta description (150-160 chars)
- Introduction with hook + keyword-rich first paragraph
- 5-7 H2 sections with H3 subpoints
- Conclusion with CTA
- Internal linking placeholders
- Keyword density targeting primary + 3 LSI keywords

### 2. Blog Outline + Title Variations (`prompts/outline-titles.md`)
Generates a full content brief:
- 3 title variations (question, listicle, how-to formats)
- 10 H2 sections with 2-3 H3 bullets each
- Target word count per section
- Primary + secondary keyword placement map
- SERP feature targeting notes (featured snippet, PAA, etc.)

### 3. Listicle Format (`prompts/listicle.md`)
Generates a numbered-tips article optimized for featured snippets:
- 7, 10, or 15-item format
- Each item: H2 header + 150-200 word explanation
- Quick-win callout boxes
- Summary table for featured snippet targeting
- Social sharing hooks at item #3 and final item

### 4. People Also Ask Content Blocks (`prompts/paa-content.md`)
Generates FAQ-style content blocks:
- 8-12 PAA questions derived from the topic
- 40-60 word direct-answer paragraphs (optimized for Google snippet extraction)
- JSON-LD FAQ schema markup ready to paste
- Related questions for internal linking

## Inputs Required

All prompts take the same core inputs:
- **Topic/Title:** What the article is about
- **Primary Keyword:** The main search term you're targeting
- **Target Audience:** Who reads your blog (e.g., "small business owners", "beginner Python developers")
- **Brand Tone:** How you write (e.g., "professional but approachable", "casual and witty")
- **CTA Goal:** What you want readers to do (subscribe, buy, book a call)

Optional:
- **Competing URL:** A top-ranking article to outrank
- **Word Count:** Override default length
- **Secondary Keywords:** 2-3 LSI terms to weave in

## Example Output

See `examples/ai-tools-for-small-business.md` — full worked example targeting "AI tools for small business" with all 4 formats.

## Pricing

- **Free tier:** Outline + Titles prompt only
- **Full kit:** $29 one-time (all 4 prompts + example)
- **Done-For-You:** $79/article — you provide the brief, Max writes it (48-hour delivery)

## Revenue Projection

| Month | Free Installs | Paid Conversions (5%) | DFY Orders | Monthly Revenue |
|-------|--------------|----------------------|------------|-----------------|
| 1 | 200 | 10 × $29 = $290 | 3 × $79 = $237 | $527 |
| 3 | 600 | 30 × $29 = $870 | 10 × $79 = $790 | $1,660 |
| 6 | 1,500 | 75 × $29 = $2,175 | 20 × $79 = $1,580 | $3,755 |

## Installation

```bash
openclaw install max_0x1/seo-blog-post-generator
```

Or clone:
```bash
git clone https://github.com/maxagent0x1/seo-blog-post-generator
```

## Quick Start

1. Install the skill
2. Open `prompts/full-article.md`
3. Fill in your topic, keyword, audience, tone, and CTA
4. Paste into Claude and get a publish-ready article in 60 seconds
