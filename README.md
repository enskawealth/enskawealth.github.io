# Compound Interest App — Enska Wealth PWA

A Progressive Web App that installs on Android and iOS home screens like a native app.

---

## Files in this package

| File | Purpose |
|------|---------|
| `index.html` | The full app |
| `manifest.json` | PWA identity (name, icon, colours) |
| `sw.js` | Service worker — enables offline use |
| `icons/icon-192.png` | App icon (Android, standard) |
| `icons/icon-512.png` | App icon (splash screens, Play Store) |

---

## Deploying to Netlify (recommended — free, takes 2 minutes)

1. Go to **netlify.com** and sign up for a free account
2. Drag and drop the entire `enska-pwa` folder onto the Netlify dashboard
3. Netlify gives you a live HTTPS URL instantly (e.g. `https://random-name.netlify.app`)
4. Go to **Domain settings → Add custom domain** and enter `enskawealth.com`

---

## Connecting your domain (Namecheap or Cloudflare)

After adding the domain in Netlify:

1. Netlify will show you two nameservers (e.g. `dns1.p01.nsone.net`)
2. Log into your domain registrar (Namecheap / Cloudflare)
3. Find **Nameservers** settings and replace them with Netlify's nameservers
4. Wait up to 24 hours for DNS to propagate (usually under 1 hour)
5. Netlify auto-provisions a free SSL certificate — HTTPS is required for PWAs

---

## How users install it

### Android (Chrome)
- Visit `enskawealth.com`
- Chrome shows a banner: **"Add Compound to Home Screen"**
- Or tap the three-dot menu → **Add to Home Screen**
- App appears on home screen with the green icon, opens full-screen with no browser chrome

### iPhone / iPad (Safari)
- Visit `enskawealth.com` in Safari (must be Safari, not Chrome)
- Tap the **Share button** (box with arrow pointing up)
- Tap **"Add to Home Screen"**
- Tap **Add** — done

---

## Updating the app

Just re-upload the files to Netlify. The service worker (`sw.js`) is set to `enska-compound-v1` — if you make significant changes, bump this to `v2` so returning users get the fresh version automatically.

---

## Promoting it on YouTube

Link in every video description:
> **Free compound interest calculator:** enskawealth.com

Add it to your channel's links panel and mention it as a free tool for viewers — this drives both channel engagement and repeat visits to the tool.
