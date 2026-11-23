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

## Conversational demo guide — 23 November 2026

The mascot now floats at the bottom-right above the mobile navigation with an “Tap me” label. It opens “Nightclub guide · Demo,” a chat bottom sheet with suggested questions and a text field. The top bar contains Menu and Notifications.

Replies are scripted using simple topic matching: getting started, people, projects, progress, sessions, messages, and passport. Replies read the current sample profile, eligible people, circle membership, tasks, and story count. Unknown questions receive a clear fallback. This is not live AI; no API, external message delivery, or credentials are involved. The conversation lasts in the current tab until refresh, and the guide only navigates—it does not claim tasks or send introductions.

The mascot hides during chat. The page has additional bottom space to keep final content reachable above the floating control. The sheet supports keyboard dismissal and focus return; its conversation and suggestions scroll independently.

The floating Tap me mascot roams diagonally and side to side across the viewport on an 18-second loop, staying inside its edges and above navigation until first opened; it then rests at bottom-right above navigation for the rest of the page session. Focus/hover stops the motion; reduced-motion preferences keep it stationary.

The assistant uses a generated teal plush monkey with mint accents and a curled tail. It is a Nightclub demo mascot, not an official OpenAI asset. The image is embedded so the HTML remains self-contained.
