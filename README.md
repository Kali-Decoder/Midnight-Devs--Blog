# Midnight-Devs--Blog

A community blog list used by https://midnight-club-lac.vercel.app/blogs.

## How To Contribute

Follow these steps to add your blog post to the site.

1. Fork this repository.
2. Clone your fork locally.
3. Create a new branch (recommended).
4. Add your blog entry to `blogs.json`.
5. Validate the JSON.
6. Commit and push your changes.
7. Open a Pull Request from your fork to this repository.

## Blog Entry Format

`blogs.json` is an array of objects. Each object must follow this format:

```json
{
  "id": 11,
  "title": "Your blog title",
  "publishedAt": "Apr 02, 2026",
  "url": "https://your-blog-link",
  "summary": "Short summary of your blog (1-2 sentences).",
  "author": "Your name or handle",
  "writerTwitter": "https://twitter.com/your_handle"
}
```

## Rules

- Keep `blogs.json` valid JSON (double quotes only, no trailing commas).
- Add your entry at the end of the array.
- Use the next available `id` (increment by 1 from the last entry).
- Make sure `url` is a direct link to your blog post.
- `summary` should be concise and readable.

## Helpful Commands

Validate the JSON:

```bash
node -e "JSON.parse(require('fs').readFileSync('blogs.json','utf8')); console.log('blogs.json is valid');"
```

## Need Help?

Open an issue or ask in the community and we will help you.
