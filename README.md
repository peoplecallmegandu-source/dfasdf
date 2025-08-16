# Steep & Sage — Tea Shop Website

A modern, full-width, responsive website for Steep & Sage — a neighborhood tea room. Built with Tailwind CSS utility classes (via CDN), Google Fonts, accessible patterns, and interactive micro-animations.

Files included

- index.html — Landing page: hero, menu with filtering, highlights, newsletter, reservation modal.
- about.html — About page: story, team, sourcing, events, and careers.
- contact.html — Contact & reservation form, contact details.

Design & implementation notes

- Full-width layout: all primary wrappers use `w-full` and the `.fluid` helper (which sets `max-width: none`) so content spans the viewport on all devices.
- Tailwind CSS is used directly from the CDN for rapid prototyping. All styling is done with Tailwind utility classes embedded in the HTML plus a few CSS variables for color/appearance.
- Google Fonts: Poppins and Merriweather (declared at the top of each HTML file in the required comment format: `{{font: Font Name}}`).
- Images: This project uses AI-requested image placeholders in the format `https://images.pexels.com/photos/8099589/pexels-photo-8099589.jpeg?auto=compress&cs=tinysrgb&h=650&w=940` for hero and product photography. Replace those with real image URLs or base64 user-provided images if you have them.
- Interactive features:
  - Menu filter (All / Hot / Iced / Herbal / Pastries)
  - Add-to-order visual feedback (demo)
  - Reservation modal with client-side handling
  - Newsletter quick subscribe (demo behavior)
  - Theme toggle persisted to localStorage
- Accessibility: forms include labels, modals close on overlay click, interactive elements are keyboard-accessible.

How to use

- To preview locally, open the HTML files in a browser. Because the project is static, most interactions are client-side demos. The contact forms post to `/api/contact` as a placeholder — integrate with your backend or email service for production.

Customizing

- Replace `{{image: ... }}` placeholders with actual image URLs (or base64 data URIs if you provide images).
- Adjust colors by editing the CSS variables in the <style> block of each HTML file.
- For production, consider compiling Tailwind locally and purging unused styles.

Notes

- This project is static by default. The contact form posts to `/api/contact` as a demo; in production hook this endpoint to an email service or backend.
- Fonts are declared at the top of HTML files in the required comment format: `{{font: Font Name}}`.

License

MIT — adapt freely for your tea shop project.
