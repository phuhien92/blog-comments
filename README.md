<p align="center">
  <a href="https://hienluong.dev">
    <img src="assets/logo.png" alt="Raymond Space logo" width="120" height="120">
  </a>
</p>

<h1 align="center">blog-comments</h1>

<p align="center">Comments for <a href="https://hienluong.dev">Raymond Space</a> · powered by <a href="https://giscus.app">giscus</a></p>

Comment storage for [hienluong.dev](https://hienluong.dev). Each blog post's comment thread lives here as a GitHub Discussion, loaded on the site through [giscus](https://giscus.app).

There is no code in this repo. It exists only so the comments can be public while the site's source repo stays private.

## How it works

- Every post on hienluong.dev shows a comment box at the bottom.
- Visitors sign in with GitHub to comment or react.
- The first comment on a post creates a Discussion here in the **Announcements** category, titled with the post's URL path.
- Later comments on that post are added to the same Discussion.

You can also reply directly in the Discussions tab, and the reply shows up on the post.

## Guidelines

Keep it on topic and civil. Spam and personal attacks will be removed, and repeat offenders blocked.

## Setup (for the maintainer)

- Repo must stay **public**, with Discussions enabled.
- The [giscus GitHub app](https://github.com/apps/giscus) must be installed on this repo.
- The site reads its settings from `SITE.comments` in the site repo's `src/config.ts`: repo name, repo ID, category, and category ID (from [giscus.app](https://giscus.app)).
- Mapping is `pathname` with strict matching. Changing a post's URL starts a new, empty thread. Don't edit or delete a Discussion's opening post either: giscus uses it to match the thread to its page.
