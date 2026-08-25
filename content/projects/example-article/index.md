+++
title = "Example Article"
description = "An example showing how to structure an article with Zola and Lagrange."
date = 2026-08-25

[taxonomies]
categories = ["Notes"]
tags = ["zola", "example"]

[extra]
image = "cover.svg"
+++

This is an example article. Replace this text with your own introduction.

## Adding sections

Use Markdown headings to organize an article. Zola generates stable heading
anchors that can be linked directly.

## Adding an image

Place an image beside this file, for example:

```text
content/projects/example-article/
├── index.md
└── photo.webp
```

Then include it with standard Markdown:

```markdown
![A useful description](photo.webp)
```

## Adding code

Fenced code blocks receive syntax highlighting:

```rust
fn main() {
    println!("Hello from Zola!");
}
```

Edit this file, rename its directory to choose a different URL slug, and remove
the example sections you do not need.
