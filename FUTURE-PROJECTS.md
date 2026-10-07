# Future Projects

A running list of projects to revisit. These entries are a backlog, not scheduled reminders.

## Mike's Pools / Adams Pools & Supplies website

- **Status:** Planned for later; no migration started.
- **Added:** October 7, 2026.
- **Website:** https://www.mikespools.us
- **Goal:** Replace paid website hosting with Cloudflare free hosting and make occasional content updates easier.

### Current situation

- The business pays only for website hosting and uses no other hosting features.
- Tim updates pricing about once a year; products and contacts occasionally change.
- The site began as a document created in Word 97.
- Tim's brother maintained it approximately 2005–2015, with no major changes.
- Tim took over about ten years ago, hand-coded an update, and added a mobile view.
- The reviewed public pages use HTML, CSS, JavaScript, and images. Their current features appear suitable for static hosting without a database.

### Proposed approach

1. Back up and inventory the complete existing site, including images and other downloadable files.
2. Put the existing site in its own GitHub repository.
3. Set up Cloudflare free static hosting with automatic deployments from GitHub.
4. Verify pages, links, images, galleries, and mobile behavior on a temporary address.
5. Preserve existing page URLs and configure both the bare domain and www before switching hosting.
6. Retire paid hosting after the replacement is verified; retain domain registration.
7. Improve the layout separately after migration, preserving the familiar site initially.

### Easier maintenance

- Store pool prices, sizes, warranties, product information, and contacts in a central, readable data file.
- Generate the relevant page content from that file so shared information only needs updating once.
- Keep the maintenance workflow simple for infrequent updates; no database or admin system is currently needed.
- Include clear instructions for editing the data and publishing changes.

### Items to review when work begins

- Check the complete asset collection against Cloudflare's then-current free-plan limits.
- Review fixed-width and table-based layouts for smaller phone screens.
- Fix shared slideshow code that can run before its target elements exist and accesses elements absent from some pages.
- Confirm current pricing, products, contacts, and business hours before any content changes.
- Confirm domain/DNS access and current hosting arrangements before cutover.
