# Agent instructions

## Git workflow

- Commit and push directly to `master`. Don't open pull requests or leave work on
  feature branches unless explicitly asked. Vercel deploys `master` to production
  (harrisonku.com).
- If a session is set up on a feature branch, push to it as well if you like, but
  always also push the finished work to `master` (`git push origin HEAD:master`,
  fast-forward only; rebase onto `origin/master` first if it has moved).
- Build locally before pushing (`bundle exec jekyll build`) to make sure the site
  still renders.
