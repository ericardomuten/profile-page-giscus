# profile-page-giscus

This repository stores the comments for my two websites. It holds no code.

The comment boxes on the sites use [giscus](https://giscus.app). Each comment thread is a
[GitHub Discussion](https://docs.github.com/en/discussions) in this repository, created
automatically the first time someone comments on a page.

## Sites

| Site | Discussion category |
|---|---|
| [ericardomuten.com](https://ericardomuten.com) (main site, Wowchemy) | `Announcements` |
| [mind.ericardomuten.com](https://mind.ericardomuten.com) (blog, Quartz) | `obsidian-quartz` |

Each site uses its own category, so pages with the same path on the two sites never share a
thread.

## How threads are matched to pages

- **Mapping: `pathname`.** A thread's title is the page path, e.g. `/talk/my-talk/`. The
  domain is not part of it.
- **Strict matching: on.** giscus finds the thread by a hash of the path stored in the
  discussion, not by GitHub's fuzzy title search.
- **Renaming or moving a page** changes its path, so the page starts a new, empty thread. The
  old thread stays here.

## Commenting

- Sign in with GitHub in the comment box on the site, or comment on the discussion here
  directly. Both end up in the same thread.
- Please keep comments on topic. I may hide or delete off-topic or abusive comments.

## For maintenance

- Both categories use the *Announcement* format, so only the repository owner and the giscus
  app can start new discussions.
- Comment box styling (light and dark themes) lives in the website repositories, not here.
