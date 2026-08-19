# 👋 Hi, I'm Yash Jangid

🎓 ECE Student @ JECRC College | 💻 Code Enthusiast | 🪵 Furniture Business Owner  
⚡ Building digital & physical products with equal passion

---

## 🚀 About Me

- 🔧 I run a **wooden furniture manufacturing business** with deep knowledge of tools, materials, and traditional craftsmanship.
- 📚 I’m pursuing **Electronics & Communication Engineering**, focused on **embedded systems, coding, and automation**.
- 🎨 Currently creating **animated content** and short-format YouTube videos for kids and spiritual seekers.
- 🔁 Balancing the **old-school grind** with **modern tech stacks**.

---

## 🛠️ Tech Stack

- **Languages:** C, C++, Python, Java, JavaScript, HTML/CSS  
- **Tools:** Git, GitHub, Adobe Express, Arduino, VS Code  
- **Domains:** DSA, OOP, Embedded Systems, Animation, Optical Communication  

---

## 📂 Projects Coming Soon

- 🚧 Smart automation for furniture systems  
- 🧠 DSA + OOP codebase for learning and interview prep  
- 📱 Spiritual animation series for YouTube  
- 💼 Portfolio website to showcase all work  

---

## 📬 Let’s Connect

- 📧 Email: yashjangid.in@gmail.com 
- 📷 Instagram: [@yashjangid](https://instagram.com/yaashshaarma)  
- 🔗 LinkedIn: www.linkedin.com/in/yashjangidin  
- 🌐 Portfolio: Coming Soon...

---

> “Old tools, new code – we build with both hands.”

---

## 🌐 About this website (site build notes)

This site is an exact structural/visual copy of the "Portavia" Framer template
(from the `Yash_Jangid` repo), with the real content swapped in. A few things
worth knowing if you (or a future Claude session) come back to edit it:

### Photos — still placeholder, swap manually
The template's original stock photos were kept as-is (per your request) so the
design keeps working. Replace these files (same filename, same aspect ratio)
in `framerusercontent.com/images/` when you have real photos:

| File | Used for |
|---|---|
| `qrxY8NagVO40NBrdhFEGgFR3PYYe606.jpg` | Hero / About portrait (front view) |
| `VRQgkdWsjawSg1qpCm45HfSY1I75d1.jpg` | About portrait (back view) |
| `IUYreEo8ON7qCLgK2tgDOW0xoI.jpg` | Small avatar next to bio |
| `w08JBQPFYIq2vr4OfcD9W6vxEug16b1.jpg` | Project cover: Smart Automation for Furniture Systems |
| `qbjsnnvP9w7UaA2syp36oUe8OSo16b1.jpg` | Project cover: DSA + OOP Codebase |
| `nTU7b0ZAdWdlqCI4mQ4tGTPpDsc0cf.jpg` | Project cover: Spiritual Animation Series |
| `2nWXrWvPxxMHSpsOkNYf8KjzP7Q16b1.jpg` | Project cover: Portfolio Website |
| `xPotMb4VrNT5rTGtXQvpYqXunU12f3.jpg`, `hleE21gbHw2Y29KULoer3tF812f3.jpg`, `RTNUbNmEH3Lg1VzA3NOYHdp3bHQ12f3.jpg`, `ZbUvwGb7xhhwmovo3t9YO4bAIGs12f3.jpg` | Testimonial avatars (John Harris, Michael Lee, Sarah Johnson, Laura Bennett) |
| `1wFj19qQG6zNr7gj3iTlH0Gdlu8c0cf.jpg`, `xmKml0E7v2iBI4zbbj0yVccaQwgc0cf.jpg` | Blog cover images |

### Social icons — platform mismatch
The template only has 3 social icon slots, styled as X/Twitter, Instagram, and
Behance. You don't have X or Behance accounts, so:
- **Instagram icon** → correctly links to `instagram.com/yaashshaarma`
- **X icon** → links to your **GitHub** instead (icon still shows the X/Twitter glyph)
- **Behance icon** → links to your **LinkedIn** instead (icon still shows the Behance glyph)

The icon graphics are injected by Framer's JS component system, not static SVG,
so they couldn't be swapped without that live JS (see below) — the destinations
are correct, just the glyphs are mislabeled. Worth a manual fix later.

### Sections kept verbatim (only "Duncan" swapped to "Yash")
Per your instruction, these still use the template's original placeholder
wording/numbers, not real ones:
- Hero tagline: "digital designer... US-based... Framer developer" (not accurate — edit if you want)
- About Me bio: same as above
- Stats row (Years of Experience / Completed Projects / Clients on Worldwide / Satisfaction Rate / Growth): all show **0** — these were animated JS counters with no real target number baked into the static page, so they froze at their starting value
- Testimonials: original quotes/names/roles (John Harris, Michael Lee, Sarah Johnson, Laura Bennett) kept as-is, just "Duncan" → "Yash" where his name appeared inside the quotes
- Blog/Insights teaser cards ("5 Design Trends...", "How to Streamline...") — kept verbatim, not clickable (see below)

### Homepage only — no About/Projects/Blog sub-pages
The template's About, Projects, and Blog pages (and the 4 project case-study
pages) turned out to have no recoverable real content — they're client-side-only
Framer routes with nothing pre-rendered. Only the homepage had real, complete
content. So this is a **single-page site**: nav links and "Browse All"/"Preview"
buttons that used to point to those pages now scroll to the matching homepage
section (`#about`, `#projects`, `#blog`) instead.

### FAQ — accordion made static
The original FAQ was a click-to-expand accordion, but the "answer" (expanded)
state was never captured in the static export — only the collapsed questions
existed. Your real answers are now shown as plain always-visible text under
each question, rather than click-to-expand, since there was no safe way to
reconstruct the missing accordion-open markup.

### ⚠️ Important: the live Framer JS bundle is intentionally removed
Framer sites re-render themselves client-side using a JS bundle hosted on
Framer's own CDN, tied to the *original* template's project ID — not something
we own or control. During testing, that script was found to **overwrite all
our edits back to the original "Duncan/Portavia" content** a few seconds after
page load. It's been removed from `index.html` so your real content stays
permanent. Side effects:
- Scroll-triggered fade-in/slide-up animations may not play (elements should
  still render at full opacity, just without the animated entrance)
- Any click-to-toggle interactivity (e.g. a mobile hamburger menu, if present)
  may not respond, since that logic lived in the removed bundle
- Fonts, the hero background video, and entrance-animation timing data still
  load from Framer's CDN (`framerusercontent.com`) — this part is fine to keep,
  it's just static assets, not the content-overwriting logic

### Contact form → mailto
The original contact form couldn't submit anywhere (GitHub Pages has no
backend, and you chose not to wire up Formspree). It's replaced with a plain
"Email Me" button linking to `mailto:yashjangid.in@gmail.com`.

