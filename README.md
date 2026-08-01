# Co-LoRA Project Page


Project page for **Co-LoRA: Collaborative Model Personalization on Heterogeneous Multi-Modal Clients** (ICLR 2026).

The site is dependency-free and can be served directly with GitHub Pages. For local preview:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Publish under the personal website

Pushes to `main` run `.github/workflows/publish-to-homepage.yml`. The workflow
copies only the static website files into this directory of the personal-site
repository:

`ta3h30nk1m/ta3h30nk1m.github.io/projects/co-lora-iclr2026/`

The resulting public URL is:

`https://ta3h30nk1m.github.io/projects/co-lora-iclr2026/`

### One-time token setup

The workflow needs permission to update the separate personal-site repository.
Create a fine-grained personal access token with **Contents: Read and write**
access to `ta3h30nk1m/ta3h30nk1m.github.io`, then add it to this repository at
**Settings → Secrets and variables → Actions → New repository secret**:

- Name: `HOMEPAGE_DEPLOY_TOKEN`
- Value: the fine-grained token

After the secret is saved, push to `main` or manually run
**Publish Co-LoRA to personal website** from the Actions tab. Presentation
source files are excluded from publication.

## Structure

- `index.html` — page content and semantic structure
- `styles.css` — responsive layout and visual system
- `script.js` — citation dialog and copy interaction
- `assets/` — supplementary figures from the paper

## Sources

- [Paper on arXiv](https://arxiv.org/abs/2506.11024)
- [Official code](https://github.com/snumprlab/fedmosaic)
