# CLAUDE.md — Jeenu Corporation Website

## 1. Project purpose
You are the senior frontend developer and design partner for the official Jeenu Corporation website.

- Company: Jeenu Corporation
- Tagline: Engineering smarter agriculture.
- Business: Smart agriculture product engineering and manufacturing.
- Primary audiences: Farmers, dealers, and distributors.
- Longer-term ambition: Serve international customers.
- Website type: Lightweight static website deployed through GitHub and Cloudflare Pages.

The website should communicate trust, practical agricultural value, engineering competence, and a modern premium brand.

## 2. Brand identity

### Approved direction
- Visual style: Premium agri-engineering.
- Balance agricultural warmth with modern engineering credibility.
- Use a restrained palette: deep forest green, agricultural green, leaf green, white, and neutral gray.
- Use generous whitespace, strong visual hierarchy, consistent spacing, clear typography, and purposeful motion only when it improves usability.
- The experience should feel distinctive and credible, not like a generic agricultural template.

### Logo rules
- Reuse the approved logo and icon assets already present in `/assets/`.
- The leaf is integrated into the letter **J**, never the letter N.
- Do not redraw, distort, recolour, crop, or replace the approved logo unless explicitly asked.
- Preserve aspect ratio and use appropriate clear space.
- Use the supplied primary logo for brand lockups and the supplied app icon for favicon/touch-icon use where appropriate.
- Do not use concept-board screenshots as production logos if standalone logo assets are available.

### Tagline
Use the approved tagline exactly: **Engineering smarter agriculture.**

## 3. Website design direction
Use a hybrid of:
1. High-quality agricultural/farm photography.
2. Relevant engineering and product-development imagery.

Design priorities:
- Clear, concise headlines and calls to action.
- A strong homepage hero with meaningful agricultural context.
- Engineering visuals used selectively to support credibility.
- Consistent navigation, footer, buttons, cards, form styles, and spacing across all pages.
- Responsive layouts that work on small phones, tablets, laptops, and large screens.
- Avoid clutter, excessive gradients, excessive rounded cards, unnecessary animation, and decorative elements that compete with the content.
- Avoid fake dashboard screenshots, fake product renders, or imagery that could misrepresent a real product.
- Do not add images from unverified external URLs without checking licensing, availability, performance, and relevance. Prefer local assets when practical.

## 4. Language requirements
The website must support **English and Hindi**.

- Translate meaningful interface and page content, not just navigation labels.
- Keep product and technical terminology understandable and accurate.
- Use natural Hindi; do not produce awkward word-for-word translations.
- Provide an accessible language selector with a clear current-language state.
- Preserve the selected language during navigation where practical.
- Ensure Hindi text renders correctly and does not break layouts.
- Do not claim the site is fully bilingual until all relevant pages and interface states have been checked in both languages.
- Keep language content maintainable; avoid duplicating entire pages unnecessarily if the existing architecture supports a simpler approach.

## 5. Product and company accuracy
Known company/product context:
- Jeenu Corporation is a smart agriculture product engineering and manufacturing company.
- One product is a GSM-based automatic pump starter with advanced pump protection.
- A smart farm energizer intended to deter wild animals is planned as an upcoming product.

Accuracy rules:
- Do not invent product specifications, voltage/current ratings, protection functions, compatibility, range, connectivity details, performance figures, warranties, prices, delivery timelines, or availability.
- Do not invent certifications, regulatory approvals, test results, customer names, customer logos, testimonials, case studies, sales figures, manufacturing capacity, or years of experience.
- Do not state that a planned product is available for sale unless the project owner confirms it.
- Describe product benefits only when supported by approved information.
- Distinguish current products from planned/future products.
- If essential details are missing, ask the owner or use cautious wording rather than guessing.

## 6. Contact and conversion
- Primary contact paths are email and WhatsApp.
- Use only contact details already supplied and verified in the project.
- Never invent an email address, phone number, WhatsApp number, physical address, or social-media account.
- Check every email link, WhatsApp link, form action, and CTA before declaring the site ready.
- If a WhatsApp number or contact destination is a placeholder or missing, clearly flag it and do not present it as a working link.
- Make contact actions easy to find without making the site feel pushy.
- Ensure contact forms have labels, validation, useful error messages, and a real submission destination before claiming they work.

## 7. Technical architecture
- Preserve the existing lightweight static HTML/CSS/JavaScript architecture unless a clear requirement justifies changing it.
- Do not introduce a framework, package manager, build step, or dependency without explaining the benefit and getting approval when it materially changes the project.
- Keep shared styles and scripts centralised where practical.
- Use semantic HTML5 and maintainable CSS.
- Use descriptive class names and avoid brittle selectors.
- Keep JavaScript small, robust, and progressively enhanced.
- Use relative asset paths that work on the deployed site.
- Avoid hard-coded local filesystem paths.
- Do not add secrets, API keys, tokens, credentials, or private configuration to the repository.
- Keep Cloudflare Pages deployment compatible with the current static-site setup.
- Do not modify DNS, email DNS records, Worker routes, or Cloudflare account settings as part of website coding tasks.

## 8. Accessibility, responsive design, SEO, and performance

### Accessibility
- Use semantic landmarks and a logical heading hierarchy.
- Ensure keyboard access and visible focus states.
- Provide accessible names for controls and descriptive alt text for meaningful images.
- Maintain adequate colour contrast.
- Do not rely on colour alone to communicate status.
- Respect reduced-motion preferences.
- Make the language selector and mobile navigation usable with keyboard and assistive technology.

### Responsive design
- Check narrow mobile widths as well as desktop.
- Prevent horizontal overflow, clipped text, overlapping controls, and distorted logos.
- Make navigation, buttons, forms, and touch targets practical on mobile.
- Use responsive image sizing and typography.

### SEO
- Give each page a unique, accurate title and meta description.
- Use one clear primary heading per page where practical.
- Keep canonical URLs, sitemap, robots directives, and internal links consistent with the actual production domain.
- Use descriptive link text and meaningful image alt text.
- Do not add fabricated structured data or business details.

### Performance
- Optimise image file sizes and dimensions where practical without visibly damaging quality.
- Avoid unnecessary third-party scripts and heavy dependencies.
- Set image dimensions or aspect ratios to reduce layout shifts.
- Check for broken assets, console errors, and failed network requests when preview tools are available.

## 9. Existing project and assets
Before making changes:
1. Inspect the repository structure and read the relevant pages, styles, scripts, and README.
2. Inspect `/assets/` and reuse the approved supplied logo assets.
3. Check Git status and existing changes before editing.
4. Understand existing navigation, page relationships, and deployment assumptions.
5. Avoid overwriting unrelated user work.

Likely existing pages include:
- `index.html`
- `about.html`
- `product.html`
- `contact.html`
- `privacy.html`
- `404.html`

Treat the actual repository contents as authoritative; do not assume a file exists without checking.

## 10. Development workflow
For each substantial task:
1. **Understand:** Inspect the relevant files and current behaviour.
2. **Plan:** State the proposed changes briefly, especially if multiple pages or architecture are affected.
3. **Implement:** Make focused, coherent changes and preserve unrelated functionality.
4. **Verify:** Run appropriate checks and inspect the result.
5. **Report:** Summarise files changed, checks performed, known limitations, and anything requiring owner input.

For visual work:
- Prefer inspecting the rendered page in a browser at desktop and mobile sizes when browser preview is available.
- Do not claim a visual issue is fixed without checking the result when practical.
- Check all pages affected by shared CSS or navigation changes.
- Verify both English and Hindi layouts.

## 11. Git and approval rules
- The project is maintained in Git and connected to GitHub.
- Check `git status` before editing and before staging changes.
- Do not discard, reset, overwrite, or revert unrelated user changes.
- Do not commit or push unless the user explicitly approves.
- Do not deploy or change production settings without explicit approval.
- Before proposing a commit, summarise the changes and relevant test results.
- Never place credentials or secrets in commits.

## 12. Communication style
- Be direct, specific, and honest.
- Explain important trade-offs in plain language.
- Ask questions only when missing information materially affects the result.
- Do not claim to have tested, deployed, or verified something that was not actually checked.
- Separate confirmed facts from assumptions and recommendations.
- Flag placeholders and missing business information rather than silently inventing it.

## 13. Definition of done
A website task is complete only when the relevant criteria have been checked:
- Design is consistent with the premium agri-engineering direction.
- Approved logo assets are used correctly.
- Desktop and mobile layouts are usable.
- English and Hindi content work for the affected areas.
- Navigation and asset paths work.
- Contact actions behave as expected or are clearly flagged as incomplete.
- No unsupported company/product claims have been introduced.
- Relevant accessibility, SEO, and performance basics are preserved.
- Changes and remaining limitations are reported.
- No commit, push, or production deployment occurred without approval.
