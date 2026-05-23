# PetalKeep Website

Static marketing site for PetalKeep, designed to be hosted on GitHub Pages.

## Local Preview

Open `index.html` directly in a browser, or run:

```sh
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## GitHub Pages Setup

1. Push this repository to GitHub.
2. In the GitHub repository, open **Settings > Pages**.
3. Set the source to **Deploy from a branch**.
4. Choose your default branch and `/ (root)` folder.
5. Save.

## Custom Domain

This repo is configured for:

```txt
petalkeep.app
```

In Porkbun, configure DNS for `petalkeep.app`:

- For an apex domain, add GitHub Pages `A` records.
- Optionally add a `www` CNAME record pointing to your GitHub Pages host.

Use Porkbun forwarding to redirect `petalkeep.com` to `https://petalkeep.app`, or point both domains at GitHub Pages and add the secondary domain in GitHub Pages settings if you prefer both to resolve directly.

GitHub's Pages settings will show the exact host target once the repository exists on GitHub.

## App Store Connect URLs

Use these values in App Store Connect:

- Support URL: `https://petalkeep.app/support`
- Marketing URL: `https://petalkeep.app`
- Privacy Policy URL: `https://petalkeep.app/privacy`

## Launch Updates

Before launch, replace placeholder links in `index.html`:

- App Store links currently use `href="#"`.
- Support uses `support@petalkeep.app`; make sure the mailbox exists.
