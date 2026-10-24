# Week 06 – Accessibility & Ethics Changes

Updated version of my Week 05 page (`lab05.html` → `lab06.html`).

## Accessibility changes
- Removed the duplicate `</head>` tag so the page is valid HTML.
- Added a viewport meta tag so the page scales properly on phones.
- Added a "Skip to main content" link for keyboard and screen reader users.
- Wrapped the article in a `<main>` landmark so assistive tech can jump straight to the content.
- Changed the menu from `<p>` tags to a proper `<ul>` list and labelled the `<nav>` ("Page sections").
- Reordered the menu so it matches the order of sections on the page (Hyperlinks before Images).
- Moved the "Special Characters" `id` onto its `<section>` to match the other sections, and added a heading for the nested list example.
- Hid the decorative smiley (☺) from screen readers with `aria-hidden="true"`.
- Table: used `scope="colgroup"` on the "Savings" header that spans three columns, and stated the currency in the caption.
- Rewrote vague link text: "email" → "email someone@swin.edu.au"; the Blackboard link now says it's an external site.
- Removed `title` attributes (keyboard and touch users can't see them); moved the image file size into the visible caption.
- Improved image alt text so it describes the photo and says the link opens the full-size image.
- Changed the special-character colour from `darkorange` (2.3:1, fails) to `#A64B00` (5.8:1, passes).
- Removed the `aside:hover { display: none; }` rule, which made content disappear when the mouse moved over it.
- Gave the thumbnail its real size (`width="160" height="120"`) so the page doesn't jump while loading.
- Darkened the definition-term colour from `green` to `#006400` (7.4:1 contrast) and darkened the list border.
- Added visible focus outlines on links, kept links underlined, and made the definition list stack on small screens.
- Added `prefers-reduced-motion` support and stopped images overflowing narrow screens.

## Ethics changes (privacy, clarity, user experience)
- Changed the Blackboard link from `http://` to secure `https://`.
- Fixed typos and unclear wording ("CCS" → "CSS", "san-serif" → "sans-serif", "will will", "logical marked", "keep you HTML") so content is clear and trustworthy.
- Labelled the external link and the image file size so users know what to expect before clicking (no surprises, respects data usage).
- Credited the photo correctly in its caption (supplied with the lab files, not taken by me).
- Added a plain-language privacy statement in the footer: no cookies, tracking or personal data collected.
- Updated the footer and page title to say this is the Lab 06 version.

## Reflection
**How can I improve accessibility for all users?**
By using correct HTML structure (landmarks, a real list for the menu, proper headings and table scopes), so screen readers can navigate the page. Adding a skip link and visible focus outlines helps keyboard users, and improving colour contrast and alt text helps users with low vision or who cannot see images.

**Are there any ethical concerns (privacy, clarity, or user experience)?**
Yes. The external link used insecure `http`, the photo was credited incorrectly, link text was vague, and there were typos that made the content less clear. A rule that hid the aside on hover also made the page confusing to use. I fixed these and added a privacy statement so users know no data is collected.

**What changes could make my design more inclusive and responsible?**
Writing clear link text, describing images accurately, crediting sources honestly, and telling users what to expect (file size, external sites). Making the layout adapt to small screens and respecting reduced-motion settings also makes the page usable for more people.