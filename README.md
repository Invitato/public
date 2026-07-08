## Invitato Public Assets

Centralized Public Assets for Invitato Web Invitation

### GitHub Pages

This repository is published as a static site via GitHub Pages, so every
asset is reachable over HTTPS by its path.

Deployment is automated by
[`.github/workflows/deploy-pages.yml`](.github/workflows/deploy-pages.yml):
on every push to `main` the entire repository is uploaded and deployed as a
Pages artifact. A `.nojekyll` file is included so files are served as-is,
without any Jekyll processing.

**One-time setup:** in the repository's **Settings → Pages**, set
**Source** to **GitHub Actions**. After that, pushes to `main` deploy
automatically (you can also trigger a run manually from the **Actions** tab).

Once live, files are available at:

```
https://<owner>.github.io/<repo>/<path-to-asset>
```

for example `https://<owner>.github.io/<repo>/logo-vendor/Glow.png`.
