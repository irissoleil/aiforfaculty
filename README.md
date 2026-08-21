# AI for Faculty — site source

Built with [Jekyll](https://jekyllrb.com/) and the
[Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) theme,
hosted on GitHub Pages.

## Writing a new post

1. Add a file to `_posts/` named `YYYY-MM-DD-a-short-title.md`.
2. Copy the front matter block from one of the sample posts already in
   `_posts/` (the `---`-fenced section at the top).
3. Set `category:` to `Field Report` or `Essay`.
4. Set `tags:` to whatever themes apply.
5. Write the post body in Markdown below the front matter.
6. Commit and push — GitHub rebuilds the live site automatically, usually
   within a minute or two.

## Editing a regular page (About, etc.)

Pages live in `_pages/`. Same idea: edit the Markdown below the front
matter, commit, push.

## Previewing changes locally (optional)

If you want to see changes before pushing:

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000` in a browser. Not required — you can
also just push and check the live site.

## First-time GitHub Pages setup

1. Create a new GitHub repository and push this folder's contents to it.
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to "Deploy from a
   branch," branch `main`, folder `/ (root)`.
4. Under **Custom domain**, GitHub should detect the `CNAME` file and
   offer to use `www.aiforfaculty.com` — confirm it, and make sure "Enforce
   HTTPS" is checked once the certificate is issued.
5. Your DNS (wherever the domain is registered) needs a `CNAME` record for
   `www` pointing at `<your-github-username>.github.io`. If that's not
   already set up from the WordPress hosting, that's the one non-GitHub
   step you'll need to handle with your registrar.
