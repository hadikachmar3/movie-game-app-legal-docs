# CineShelf — public pages

Public support and legal pages for the **CineShelf** Android app.

- [Home](index.md)
- [Delete your account](account-deletion.md)

Contact: coding.with.hadi@gmail.com

---

## How to publish this (one time)

The contents of this folder are self-contained. Copy them to the **root** of a
new, **public** GitHub repository — for example `cineshelf-site`.

```bash
# from inside this folder
git init
git add .
git commit -m "Add CineShelf public pages"
git branch -M main
git remote add origin https://github.com/<your-username>/cineshelf-site.git
git push -u origin main
```

Then enable GitHub Pages:

1. Open the new repository on GitHub → **Settings → Pages**.
2. Under **Build and deployment → Source**, choose **Deploy from a branch**.
3. Branch: **`main`**, folder: **`/ (root)`**. Save.
4. Wait for the build to finish (a minute or two).

Your URLs will be:

```text
https://<your-username>.github.io/cineshelf-site/
https://<your-username>.github.io/cineshelf-site/account-deletion
```

**Verify both URLs in a private/incognito window.** Google's reviewer must be
able to open them without signing in to GitHub and without installing the app.
If the repository is private, the pages will not load and the submission will
be rejected.

## Where these URLs go

| URL | Play Console location |
|---|---|
| `.../account-deletion` | App content → Data safety → account deletion |
| Privacy policy URL | Store settings → Privacy policy |

Record both in `docs/release/PLAY_CONSOLE_ANSWERS.md` in the main repository.

## Keep it accurate

If the in-app deletion path ever changes, update `account-deletion.md` to
match. Google checks that the described steps work in the shipped app.
