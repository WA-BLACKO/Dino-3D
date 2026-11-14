# Dino Rush — Wildlife Update

## Play and publish

Upload the contents of the Project Github folder to your GitHub repository root.
The entry page is index.html. All runtime files are together, with relative links.
Enable GitHub Pages for that repository using the main branch and root folder.
Open Run-Dev.html directly for the bundled offline edition.

## Controls

- Computer keyboard: ↑ to jump, ↓ to crouch, and ← or → to change lanes.
- Phone or tablet: swipe up to jump, down to crouch, and left or right to change lanes.
  Swipe on the game view once the countdown finishes.

The hint in the main menu footer and countdown follows the active input method
and is available in English and Sinhala.

## Worlds

- Desert: anchored mesas, thin warm clouds, ribbed flowering cacti and feathered raptors.
- Autumn Forest: layered tree crowns, leafy berry shrubs and warm-breasted woodland birds.
- Snowfield: pale clouds, snowy pines, miniature snowy ridges and snowy owl-like birds.
- Volcanic Ash and Cyber City: temporarily unavailable. Selecting either displays a
  bilingual notice while keeping the current playable map. Old saved preferences
  for these two maps safely fall back to Desert. Their source assets are retained.

Birds now have layered primary and secondary feathers, fan-shaped tails, eyes,
beaks, tucked feet and a slower flap/glide cycle. Snowballs are replaced by
asymmetric peaks with white ridges and blue shaded creases. Cacti have curved ribs,
spines and small flowers. Bushes have visible woody branches, individual leaves
and berries; trees have layered crowns.

Distant mountains remain anchored on the horizon. Near scenery wraps behind the
camera and beyond the fog. Clouds drift slowly, independently of running speed.
Ground obstacle collision dimensions follow each model; every obstacle is jumpable.

## Editable source

Source-Code.zip contains the updated TypeScript project and tests. It is optional
for hosting; keep it if you want to edit the game later.

In the source folder:

    npm ci
    npm run dev

Build the hosted and offline versions:

    npm run build
    node scripts/github.mjs

Run tests with Node 24 or newer:

    node --test tests/*.test.ts

