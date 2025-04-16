---
layout: default
title: Contributing
permalink: /contributing/
---

# 🎕️ Contributing to the Campfire Resources Site

Thanks for your interest in improving this collection of Cub Scout skits, songs, and stories! Whether you're fixing typos, adding content, or just testing things out — we're glad you're here.

This project runs on [Jekyll](https://jekyllrb.com) and is hosted with GitHub Pages. Content is written in Markdown with front matter metadata in YAML.

---

## ✨ Content Guidelines

This site is intended for **Cub Scout audiences**, ranging from **Lion (Kindergarten)** to **Webelos (5th Grade)**. Please follow these guidelines when submitting content:

- ✅ Keep it age-appropriate (no sarcasm, adult jokes, or cultural references young kids won’t get)
- ✅ Avoid skits or stories involving water, bodily fluids, or humiliation
- ✅ Jokes should be understandable by kids ages 5–11 (puns are great — but explain them if needed!)
- ✅ Group participation is encouraged (especially for shy Scouts)
- ✅ Include helpful notes about staging, narrator options, and how to adapt the content for various ranks
- ✅ Bonus: Include motions, actions, or call-and-response elements!

---
## Organizing Content
Stories, skits and songs should go in their respective `_stories`, `_skits`, `_songs` folders.  They must has the apprpriate type in their yaml front matter in order to apply the right header.

You can add a new type of campfire content by adding a folder (must start with `_` for Jekyll) and adding a layout to `_layouts` named after that type.

All content files should be named with dashes (`-`) between word.  For example: `the-invisible-bench.md`

---

## 📋 YAML Front Matter & Markdown Format

Each file must begin with a YAML front matter block (`---`) that defines its properties. Here are examples by content type:

### 📝 Skits

```yaml
---
layout: skit
title: "The Invisible Bench"
age_groups:
  - Wolf
  - Bear
number_of_scouts: "3+"
props:
  - Bench (can be imaginary)
  - "Optional: Name tag for narrator"
themes:
  - Humor
  - Physical Comedy
tags:
  - campfire
  - audience-favorite
---
```

### 🎵 Songs

```yaml
---
layout: song
title: "The Moose Song"
age_groups:
  - Lion
  - Tiger
themes:
  - Movement
  - Humor
tags:
  - repeat-after-me
  - action-song
tune: "Traditional"
instructions: |
  - Repeat each line after the leader.
  - Add silly motions for each verse.
  - End with a loud, dramatic final line.
---
```

### 📖 Stories

```yaml
---
layout: story
title: "The Unknown Scout"
age_groups:
  - Bear
  - Webelos
storyteller: "Adult"
length: "Short"
tone:
  - Inspirational
  - True Story
tags:
  - scout-spirit
  - helpful
---
```

Use :::line, :::action, and :::ask to mark storyteller lines, actions, and audience questions. End each block with :::.

### ✅ Notes:

- Use `- "Optional:..."` in `props:` to flag optional items (quotes are required).
- Use `|` to create multi-line blocks for fields like `instructions:`
- Markdown formatting inside content (after the front matter) is fully supported:
  - Use `**bold**` or `_italic_`
  - Use `> ` for blockquotes (e.g., dialogue)
  - Use headings (`##`) to structure long stories or scripts
  - Wrap callouts or notes in `**Narrator:**`, `>`, or custom styles

## Automatically Formatting Content
If you are pulling content from another source, ensure that your have permission and you follow any attribution requirements.

An easy way to import content from other sources is to use ChatGPT or another generative AI model to convert the content into the final markdown+yamnl format.  The following system prompt has been successful but your mileage may vary depending on model.

````text
Format the following Cub Scout skit, song, or story for a website that catalogs age-appropriate campfire content. Use YAML front matter and Markdown. Include fields like title, age groups, number of scouts (for skits), props, themes, tags, and a well-formatted script. Follow this example:

```markdown
---
layout: skit
title: "The Viper is Coming"
age_groups:
  - Tiger
  - Wolf
  - Bear
number_of_scouts: "2–4"
props:
  - Broom
  - "Optional: Mop bucket"
themes:
  - Humor
  - Wordplay
tags:
  - audience-favorite
  - groaner
  - misdirection
---

## 🐍 Skit: The Viper is Coming

**Narrator:** A group of scouts are sitting around when they hear a whisper…

> Voice (offstage): “I am the Viper… I vill come in FIVE minutes…”

Scouts react, get more nervous as countdown continues.

> “I am the Viper… I vill come in ONE minute…”

Finally, someone knocks and enters with a bucket and broom:

> “I am the Viper! I’ve come to vipe your vindows!”
```

Now here is the content to format:

(Paste skit, song, or story here)
````

---

## 🔍Searching
[search.json](https://github.com/danielrischar/campfire-resources/blob/main/search.json) defines what properties are searchable by converting them to json.  If you add a new property to yaml front matter, you need to add it here to make it searchable.

When GitrHub pages deploys, Jekyll will generate a json file for all content based on thes tags, that's how the searching is then performed on the frontend.

---

## 🔧 Git Clone Workflow for Contributing

If you're new to Git or GitHub, here’s a simple way to make and submit changes:

### 🛠️ 1. Clone the repo

```bash
git clone https://github.com/danielrischar/campfire-resources.git
cd campfire-resources
```

### 🌿 2. Create a new branch

```bash
git checkout -b add-my-awesome-skit
```

### ✍️ 3. Make your changes

Add or edit files in `_skits/`, `_songs/`, or `_stories/`. Preview locally with:

```bash
bundle install
bundle exec jekyll serve
```

View at [http://localhost:4000](http://localhost:4000)

### ✅ 4. Commit your changes

```bash
git add .
git commit -m "Add new skit: The Talking Backpack"
```

### 🚀 5. Push your branch

```bash
git push origin add-my-awesome-skit
```

### 📬 6. Open a pull request

Go to your repo on GitHub, and it will prompt you to "Compare & Pull Request." Describe your contribution and submit the PR!

---

## 💬 Questions? Suggestions?

Feel free to open an issue or ping the maintainer with any ideas or formatting help. We're always happy to improve the site and support new contributors!

---

Thank you for helping bring laughter, learning, and Scout spirit to campfires everywhere. 🔥