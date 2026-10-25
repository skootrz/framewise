# Publishing this support repo

One-time steps (this file is excluded from the Pages site).

1. On GitHub, create a new **public** repository named `framewise` under
   `skootrz`. Leave it empty (no README, license or .gitignore).
2. Push this folder (the first commit is already made):

   ```sh
   cd ~/Documents/GitHub/framewise
   git remote add origin https://github.com/skootrz/framewise.git
   git push -u origin main
   ```

3. **Settings → General → Features:** make sure **Issues** is checked. Uncheck
   Wikis, Projects and Discussions if you don't want them.
4. **Settings → Pages:** Source **Deploy from a branch**, branch `main`,
   folder `/ (root)`, then Save. After a minute or two the site is live at
   <https://skootrz.github.io/framewise/>.
5. Check the three URLs load:
   - Support: <https://github.com/skootrz/framewise>
   - Privacy: <https://skootrz.github.io/framewise/privacy/>
   - New issue picker: <https://github.com/skootrz/framewise/issues/new/choose>
6. Optional: **Settings → General → Features → Issues → Set up templates** is
   not needed; the templates in `.github/ISSUE_TEMPLATE/` are picked up
   automatically. Add `bug`/`enhancement` labels if GitHub didn't create them.

## App Store Connect

- **Support URL:** `https://github.com/skootrz/framewise`
- **Privacy Policy URL:** `https://skootrz.github.io/framewise/privacy/`

Use the same two URLs in Microsoft Partner Center.

## Keeping the privacy policy in sync

The source of truth is `video-metadata-app/PRIVACY.md` in the private repo.
When it changes, copy it here below the front matter block at the top of
`PRIVACY.md` and push.
