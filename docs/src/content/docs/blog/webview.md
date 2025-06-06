---
title: Revamping the views...
date: 2025-01-23
authors:
  - pelikhan
tags:
  - react
  - webview
  - vscode
canonical_url: https://microsoft.github.io/genaiscript/blog/webview
description: Announcing the new GenAIScript view.
cover:
  alt: The image illustrates a split screen in an 8-bit style, contrasting two
    environments for the GenAIScript interface. On the left, a computer monitor
    shows the interface with interactive elements like mermaid diagrams and math
    notations. On the right, a standalone web browser presents the same
    interface. The composition is framed with a simple, geometric design using
    five accent colors, creating a vibe of technological progress in a corporate
    context.
  image: ./webview.png
excerpt: We've enhanced the GenAIScript experience by moving beyond Visual
  Studio Code's default Markdown preview. Our new custom webview not only
  supports additional formats like mermaid diagrams and math but also allows you
  to access and run scripts directly in your browser or other webview-compatible
  apps. The transition is seamless, with options to test this alongside the
  existing features. Explore these updates for a more interactive and flexible
  workflow.

---

In the past, our Visual Studio Code visualization has relied on the built-in Markdown preview feature. It's been working great but sometimes it's not enough. We wanted to provide a more interactive experience for our users. So we decided to build a custom webview for GenAIScript.

Rebuilding the view also gives us more control on supporting the rendering of various markdown subformats like mermaid diagrams, annotations, math, ...

![A screenshot of the GenAIScript view.](./webview.png)

:::note

As we test and migrate to the new view, the old `Output`/`Trace` menu items are still available from the status bar menu.

:::

## Accessing the view outside of Visual Studio Code

As a result of this change, you can now access the GenAIScript view outside of Visual Studio Code. This means you can now **run** your scripts in a browser or any other webview-capable application.

Launch the [serve](/genaiscript/reference/cli/serve) command from the [cli](/genaiscript/reference/cli) to start the server and follow the instructions to open the view in your browser.

```sh
genaiscript serve
```
