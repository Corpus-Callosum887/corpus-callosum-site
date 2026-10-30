# Corpus Callosum website (v01)

Static site for GitHub Pages. Pages: home, Hello Faces, privacy policy, support, delete account.
Custom domain: corpuscallosum.studio (set by the CNAME file).

## v07 — invite pages and app links
- `404.html` doubles as the invite page: GitHub Pages serves it for any unknown address, so
  `/l/CODE` (Pass the Laugh) and `/s/CODE` (Face Squad invite) fill themselves in from Supabase.
  It speaks the visitor's phone language (7 languages). Store buttons switch on at launch:
  set APP_STORE_URL and PLAY_URL at the top of its script.
- `.well-known/apple-app-site-association` and `.well-known/assetlinks.json` let iPhone and Android
  open those links straight in the app when it's installed. Replace YOUR_TEAM_ID and the two
  SHA-256 fingerprints before pushing.
- `.nojekyll` makes GitHub Pages serve the `.well-known` folder.
