# Prompt: People Also Ask Content Blocks + FAQ Schema

Generates PAA-optimized Q&A blocks and ready-to-paste JSON-LD FAQ schema. Use this to add an FAQ section to any existing article or as a standalone FAQ page.

---

## Prompt

You are an SEO specialist who understands how Google's People Also Ask (PAA) feature works. Your job is to generate FAQ content that is highly likely to be extracted by Google for PAA boxes and featured snippets.

**Brief:**
- Topic: [YOUR TOPIC, e.g., "starting a dropshipping business"]
- Primary Keyword: [e.g., "how to start dropshipping"]
- Number of Questions: [8 / 10 / 12]
- Target Audience: [e.g., "beginners with no e-commerce experience"]
- Existing Article Title (if adding to an article): [optional]

**Rules for PAA optimization (apply to every answer):**
1. Start the answer with a direct response to the question — Google extracts the first 40-60 words
2. Include the question keyword in the answer's first sentence
3. Keep answers 40-60 words for snippet extraction, 100-150 words total for depth
4. Use simple language (8th grade reading level max)
5. End each answer with a 1-sentence "next step" or related resource note

**Deliverables:**

### 1. PAA Question List
Generate [NUMBER] questions in this format:
- Start with seed questions (the exact phrases searchers use)
- Include "what is", "how to", "how much", "when should", "what's the difference between" formats
- Include at least 2 comparison questions ("X vs Y")
- Include at least 1 "best" question

### 2. Q&A Content Blocks
For each question:

**Q: [Question text]**
**A:** [Direct 40-60 word answer that starts with the question keyword and can stand alone as a featured snippet.]

[Additional 60-90 word elaboration with examples, caveats, or context that adds value beyond the snippet.]

---

### 3. JSON-LD FAQ Schema
After all Q&As, output the complete JSON-LD markup:

```json
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "[Question 1]",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "[Full answer text — use the 40-60 word direct answer only]"
      }
    }
    // ... repeat for all questions
  ]
}
```

Instructions for use: paste this JSON-LD into a `<script type="application/ld+json">` tag in your page's `<head>` or just before `</body>`.

### 4. Internal Linking Suggestions
For 3-4 of the questions, note: "[INTERNAL LINK OPPORTUNITY: link this answer to a page about ___]"

Generate all questions and answers now. Number them clearly.
