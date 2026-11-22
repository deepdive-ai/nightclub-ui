# Nightclub — Mobile prototype

Open `NIGHTCLUB_MOBILE_MASCOT_GP.html` in a browser. This is a self-contained mobile web prototype, not an installed native app. All illustrations are embedded. On desktop it displays a phone-width layout; on a phone it fills the screen width up to 480px.

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

## Mascot edition

An original lavender puzzle-piece mascot sits between Menu and Notifications. Its “Tap me!” label opens a navigation guide with links to people, builds, sessions, and the passport. This is a local navigation helper, not an AI service. The collaborator card has four generated puzzle-piece characters.
