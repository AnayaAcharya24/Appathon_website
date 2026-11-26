# Project memory

## Product intent & audience

- APPATHON — appears to be a hackathon or app competition platform.
- Homepage showcases Social Impact, Prizes & Recognition (First Prize, Second Prize, Participation Certificate), and Important Announcements sections.
- Audience: prospective participants; tone is premium, futuristic, polished.

## Brand personality & voice

- Vibrant, luminous, cinematic — not dark, flat, or excessively neon.
- Premium and futuristic visual language with glassmorphism and animated light effects.
- Purple-dominant palette: Electric Purple `#7024D8`, Vivid Violet `#A64AFF`, Soft Lavender `#C9A4FF`.

## Visual design & UX direction

- Animated video background in the combined Social Impact / Prizes / Announcements area: brightened, saturated, with flowing curved light ribbons, layered radial glows; dark overlay reduced for visibility while preserving text contrast.
- Glassmorphism cards: translucent dark-purple fill, backdrop blur, diagonal sheen reflection, enough transparency to reveal background animation through cards.
- Animated gradient borders on all cards: ~2px, three-colour (purple/violet/lavender) travelling gradient with gentle breathing glow and subtle light highlight; no rapid flashing.
- First Prize card has slightly stronger/faster glow than the other four cards, which remain consistent in brightness.
- Hover: slight upward lift, brighter gradient glow, light-sweep reflection, smooth enter/exit transitions.
- Desktop layout: Prizes & Recognition and Important Announcements side by side; responsive on mobile.
- Accessibility: `prefers-reduced-motion` respected for all animations.
- Components/patterns: Tailwind utility classes for styling; Lucide React for icons; `@/` path alias for imports.

## Decisions, constraints & rationale

- Prize cards (First, Second, Certificate) are themselves individual glass cards rather than an outer glass panel wrapping them — ensures consistent border animation across all five cards.
- Removed opaque award-card fill and its `::before`/`::after` pseudo-elements to avoid double-borders with the unified glass border.
- Scope strictly limited to the combined Social Impact / Prizes / Announcements area; navigation, hero, other sections/pages, and global styles untouched.
- Existing content, text, images, icons, links, card dimensions, spacing, and layout preserved.

## Open questions & assumptions

- No explicit mention of other pages or routing structure beyond homepage.
- Background video source and implementation details not specified; assumed existing video element was enhanced rather than replaced.
- Exact card component names/paths not yet catalogued — may need mapping if further card changes are requested.