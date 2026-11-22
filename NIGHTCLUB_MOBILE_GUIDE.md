# Nightclub — Mobile prototype

Open `NIGHTCLUB_MOBILE_GP.html` in a browser. This is a self-contained mobile web prototype, not an installed native app. All illustrations are embedded. On desktop it displays a phone-width layout; on a phone it fills the screen width up to 480px.

## Mobile design

- Compact welcome with the “nightclub” headline in pink handwriting, GP persona, and subtle illustrated backdrop.
- One prominent collaborator-discovery card featuring four illustrated puzzle-piece characters, followed by a compact two-column shortcut grid.
- Top bar: Menu on the left and Notifications on the right. Demo controls are inside the menu; the GP avatar remains beside the welcome area.
- Persistent Home, Discover, Build, Messages, and Profile navigation.
- Existing deeper sections reachable through cards, contextual links, and the menu.
- Native HTML dialogs styled as bottom sheets, larger input text, and touch-friendly controls.
- A local build-progress summary linked to the existing demo task state.
- Safe-area padding for phone navigation and reduced-motion support.

## Try the prototype

1. Tap **Explore your four** to view sample collaborators.
2. Open the menu for **Connections**, where you can accept an incoming sample request or simulate acceptance of your outgoing request.
3. Open **Messages** to try a local conversation.
4. Open **Build** to inspect tasks and review sample work.
5. Use **Profile** to edit the GP sample persona.
6. Home shortcuts lead to opportunities, sessions, and your contribution passport.

## Scope

The desktop HTML is unchanged. This version has its own browser-storage key, so its demo state is separate from the desktop edition. All accounts, messages, applications, RSVPs, reports, and publication actions remain illustrative local simulations. No real backend, payment, authentication, or messaging service is connected.

Fonts depend on what the recipient has installed. This prototype is for interaction and design review; it is not a production app or an accessibility certification.

## Verification

JavaScript syntax checked successfully. All five bottom tabs were exercised at 390px width. The introduction bottom sheet was visually checked. All 16 routes were checked for document overflow at 320px width and reported none. Browser error log was empty during these checks. These checks do not replace testing on physical iOS and Android devices.

## Mobile UI finishing pass — 22 November 2026

- The current header keeps the branding beside GP, the welcome centered, and the uppercase growth tagline with a dark green sketch highlight.
- Press feedback is shared across links and enabled buttons. Keyboard focus remains visible; reduced-motion preferences disable decorative motion.
- The profile touch target is at least 44 × 44 px. Form text uses 16 px to reduce automatic zoom on phones. Long welcome names can wrap rather than overflow.
- Menu opens with keyboard focus, closes with Escape or an outside click, and returns focus on Escape. Bottom-sheet dialogs restore focus on dismissal.
- Menu → Demo controls includes Normal, Loading, Two available, No matches, Offline, and Load error. Loading, failure, and retry examples apply to Discover, Find Your Four, and Build.
- Loading is deliberately simulated; “Finish loading demo” returns to normal content. No real network requests or messages are made.

Validation scope: browser layout checks across all 16 routes at 320, 390, and 430 px; targeted search, profile sheet, introduction consent validation, save/unsave feedback, deliverable details, and passport checks. This is prototype QA, not a claim of comprehensive accessibility certification or real-device/backend testing.
