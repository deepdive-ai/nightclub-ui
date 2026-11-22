# Nightclub Frontend — Darker Cards Edition

## Deliverable

**Prototype:** `NIGHTCLUB_FRONTEND_BUBBLEGUM_DARKER_CARDS_GP.html`

Download the HTML file and open it in Safari, Chrome, or Edge. All styles, JavaScript, and illustration assets are embedded. Send this single HTML file as an attachment; no installation, internet connection, or local server is required to use the demo. A local file link on the creator’s computer is not a public website URL.

This edition is a separate copy of the bubblegum prototype. The preceding version is preserved.

## Design direction

A minimal, illustrated community workspace with translucent glass panels and darker pastel navigation cards. The page uses a soft-white background and a faint community-building illustration. The illustrations depict collaborators, ideas, and shared work.

- Sample profile name: **GP**.
- Headline: **Small steps. Good company.**
- Headline color: bubblegum pink, `#ED83B5`.
- Handwriting font stack: Chalkboard SE, Chalkboard, Comic Sans MS, Comic Sans, cursive. The actual typeface depends on installed fonts; no font file is embedded.
- Page background: soft white, `#FCFCFA`.
- Background illustration: 18% opacity, reduced saturation.
- Tagline: **MADE TO BUILD TOGETHER**, without the starburst symbol.
- Greeting: “Hey GP. Find your people, make something useful, and see where it takes you.” Each character cycles through pink, purple, teal, and berry shades. A single accessible label supplies the complete sentence.
- Main button: **Find your next step**, light purple `#DFD0F3` with plum text `#543574`; scrolls to the card directory.

## Darker card palette

These are the CSS base colors. Transparency, background artwork, and glass highlights affect their final rendered appearance.

| Card | Color family | CSS background |
|---|---|---|
| Find your missing pieces | Teal | `#7ABCAFDD` |
| A door your work could open | Peach | `#E8A786E8` |
| Make something real | Golden yellow | `#DFC16FE8` |
| Learn it. Build it. | Lavender | `#B29ACFE8` |
| From the build floor | Sage | `#A6C292E8` |
| Let your work speak | Rose | `#D9A0B2E8` |

The final two hexadecimal digits specify opacity. Card headings use warm dark text `#352A24`; descriptions and labels use `#493A32`.

## Homepage behavior

Each complete card is a clickable link that opens the corresponding application section.

| Card heading | Destination | Purpose |
|---|---|---|
| Find your missing pieces | Find Your Four | Explore complementary sample collaborators and request an introduction. |
| A door your work could open | Opportunities | Explore sample pilot, freelance, and career opportunities. |
| Make something real | Build Missions | Review tasks, submit sample contributions, and acknowledge deliverables. |
| Learn it. Build it. | Sessions | Explore learning sessions and record a local RSVP. |
| From the build floor | Discover, build-update feed | Read and contribute to a finite sample community feed. |
| Let your work speak | Builder Passport | Preview contribution stories and demonstrate consent-based publication. |

Secondary links provide access to Connections, Messages, Circles, Resources, Builder Persona, Membership, and Settings. The menu exposes the broader application navigation. Presenter controls provide sample scenarios and a guided tour.

## Layout and effects

- Desktop: two columns of large cards.
- Phone: one column with compact spacing and smaller illustrations.
- Cards: rounded corners, translucent colored fills, frosted blur where supported, highlights, and soft shadows.
- Hover: subtle card lift and 3D tilt, with a small illustration movement.
- Reduced-motion preference disables the hover motion.
- Fallback backgrounds preserve the card treatment when backdrop blur is unavailable.
- Keyboard focus indicators and semantic links support navigation.

## Existing prototype sections

The HTML retains 16 routes: Home, Find Your Four, Discover, Connections, Messages, Circles, Build Missions, Builder Passport, Sessions, Opportunities, Resources, Notifications, Membership, Settings, Builder Persona, and Admin Preview.

The demo includes persona editing and goal allocation validation; opt-in introductions and simulated acceptance; local messaging between accepted sample connections; circle proposals; deliverable review; contribution stories; session RSVPs; opportunity interest; resource notes; notification states; membership controls; safety controls; and presenter scenarios.

## Data and limitations

This is an HTML/CSS/JavaScript frontend prototype using fictional sample data. It has no live backend, authentication, payment processing, real message delivery, or public publishing service. Actions such as sending, applying, reporting, and publishing are local simulations.

Demo changes are saved in the current browser when local storage is available. Different recipients do not share data. This darker-card copy retains the preceding bubblegum edition’s storage key, so previews served from the same web origin can share demo state. Local-file storage behavior varies by browser.

The headline’s installed-font fallback and translucent backgrounds may render differently across devices. This darker palette is a design iteration; a full contrast, assistive-technology, and cross-browser audit has not been completed.

## Presentation instructions

1. Open the HTML in a browser.
2. Use the top demo-controls button to reset sample data if needed.
3. Show the headline and greeting, then select **Find your next step**.
4. Click a card to demonstrate its corresponding section.
5. Explain that all people and actions are illustrative and local.

## Sharing

Send **NIGHTCLUB_FRONTEND_BUBBLEGUM_DARKER_CARDS_GP.html** for the interactive prototype and this Markdown document for the design and functionality description. The HTML contains the artwork; recipients do not need a separate assets folder.
