# Octeum SentrX - GitHub Status Page

GitHub Status Page for Octeum SentrX using an open-source status page, powered entirely by GitHub Actions, Issues, and Pages.

![screenshot](.github/screenshot.png)

# Usage

## Reporting your incident

1. Go to issues tab
2. Create a new label named `incident`
3. Create a issue
4. Add the label `incident` to the issue

# How it works

- Hosting
  - GitHub Pages is used for hosting the status page.
- Monitoring
  - Github Workflow will be triggered every 2 Hr (Configurable) to visit the website.
  - Response status is compiled and the site is rebuild with the new information.
- Incidents
  - Github issue is used for incident management.

# Credits

<a target="_blank" href="https://icons8.com/icon/14835/heart-monitor">Heartbeat</a> favicon by <a target="_blank" href="https://icons8.com">Icons8</a>

Project is mainly inspired by [mehatab/fettle](https://github.com/mehatab/fettle).
Main difference between this project and fettle are:

- This project was built in SvelteKit.
- It doesn't commit the status log, instead it is stored as an artifact.
- You can set up your health urls as a secret by using [`repository secrets`](https://docs.github.com/en/actions/security-for-github-actions/security-guides/using-secrets-in-github-actions).
- You can host it in any GitHub pages. You [don't need a custom url](https://github.com/mehatab/fettle/issues/20).
