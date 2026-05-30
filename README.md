# PetalKeep Website

Static marketing site for PetalKeep, designed to be hosted on GitHub Pages.

Repository: `https://github.com/brianjmurray/petalkeep-site`

## Local Preview

Open `index.html` directly in a browser, or run:

```sh
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## GitHub Pages Setup

GitHub Pages is enabled from the `main` branch and `/ (root)` folder.

## Custom Domain

This repo is configured for:

```txt
petalkeep.app
```

In Porkbun, configure DNS for `petalkeep.app`:

- `A` record: host `@`, answer `185.199.108.153`
- `A` record: host `@`, answer `185.199.109.153`
- `A` record: host `@`, answer `185.199.110.153`
- `A` record: host `@`, answer `185.199.111.153`
- `CNAME` record: host `www`, answer `brianjmurray.github.io`

Use Porkbun forwarding to redirect `petalkeep.com` to `https://petalkeep.app`, or point both domains at GitHub Pages and add the secondary domain in GitHub Pages settings if you prefer both to resolve directly.

After DNS propagates, return to **Settings > Pages** in GitHub and enable **Enforce HTTPS**.

## Email

The site currently links to `support@petalkeep.app`.

For App Store submission, either:

- Create a free Porkbun email forward from `support@petalkeep.app` to your personal inbox if receiving support mail is enough.
- Create a hosted mailbox for `support@petalkeep.app` if you want replies to come from the custom PetalKeep address.

Forwarding is enough for App Review, but a hosted mailbox looks more polished for customer support.

## App Store Connect URLs

Use these values in App Store Connect:

- Support URL: `https://petalkeep.app/support`
- Marketing URL: `https://petalkeep.app`
- Privacy Policy URL: `https://petalkeep.app/privacy`

## Launch Updates

Before launch, confirm support uses `support@petalkeep.app` and make sure the
mailbox exists.
