# Lagrange for Zola

This is a Zola port of [Lagrange](https://github.com/LeNPaul/Lagrange), the
minimalist Jekyll theme by Paul Le.

## Setup

Set the theme and core metadata in your site's `config.toml`:

```toml
theme = "lagrange"
title = "My site"
description = "Notes and projects"
author = "Your name"
compile_sass = true

[extra]
posts_section = "posts/_index.md"
header_bio = "A short introduction shown in the site header."
menu = [{ name = "Writing", url = "/posts" }]
social = [{ name = "GitHub", icon = "github", url = "https://github.com/user" }]
older_page = "Older"
newer_page = "Newer"
read_more = "Read more"
post_date_prefix = "Written on"
sharing_button_prompt = "Feel free to share!"
related_posts = "You may also enjoy:"
hide_post_date = false
hide_post_share = false
hide_related_posts = false
disqus_shortname = ""
google_analytics_id = ""
```

Configure the root section for the homepage:

```toml
+++
title = "Home"
template = "index.html"
+++
```

Configure `content/posts/_index.md` as the post archive:

```toml
+++
title = "Writing"
sort_by = "date"
template = "section.html"
page_template = "post.html"
paginate_by = 5
paginate_path = "page"
+++
```

Post images may be absolute URLs, root-relative static paths, or colocated
bundle assets set as `image` under `[extra]`.
