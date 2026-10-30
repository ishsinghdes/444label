# 444 Records

Static music website for 444 Records.

## Upload to a new GitHub repository

1. Extract this ZIP.
2. Open your new repository, choose **Add file → Upload files**, and upload the extracted contents. Keep `index.html` at the repository root.
3. Include the `.github` folder. If your file picker hides it, show hidden files or upload it using GitHub Desktop.
4. Under **Settings → Pages → Build and deployment**, choose **GitHub Actions** as the source.
5. Open **Actions → Deploy GitHub Pages → Run workflow** if deployment has not started automatically.
6. The Pages link appears under **Settings → Pages** after deployment succeeds.

You can also publish directly from the default branch: choose **Deploy from a branch**, select your default branch and **/ (root)**, then save. The workflow is optional with that method.

## Notes

- No build or package installation is required.
- Use a web server to preview locally; opening index.html directly does not support the catalog fetch and JavaScript modules.
- Stream estimates and verified YouTube data are stored separately in `catalog.json`. Estimated headline totals use artist-provided Spotify and Apple figures. Floating per-song estimates use the configured multiplier.
- The daily refresh task attached to the original Sites hosting does not transfer to GitHub Pages. Update `catalog.json` and commit changes to refresh the GitHub-hosted data. The page checks that file every 24 hours while open.
- YouTube playback depends on browser autoplay rules and embedding availability. Actual beat analysis is not available through YouTube; motion follows playback state with a rhythmic animation.
- Newsletter requests use FormSubmit for 444recordsonly@gmail.com. Inbox activation is required before delivery works.
- Some artist/platform links open searches where direct profiles were not verified.
- The custom domain 444.records is not configured in this package. Purchase it and configure GitHub Pages when ready.
