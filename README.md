# RazorComponents.Markdown

![CI](https://github.com/StardustDL/RazorComponents.Markdown/workflows/CI/badge.svg) ![CD](https://github.com/StardustDL/RazorComponents.Markdown/workflows/CD/badge.svg) ![License](https://img.shields.io/github/license/StardustDL/RazorComponents.Markdown.svg) ![downloads](https://img.shields.io/nuget/dt/StardustDL.RazorComponents.Markdown)

Razor component for Markdown rendering.

## Features

Most features are based on Markdig.

- Abbreviations
- Auto identifiers
- Citations
- Custom containers
- Definition lists
- Emphasis extras
- Figures
- Footers
- Footnotes
- GridTables
- Mathematics
- Media links
- Pipe tables
- Task lists
- Diagrams, flowcharts
- Auto links
- Smarty pants
- Emoji
- Code highlighting

## Usage

1. Add the newest package on NuGet.

See https://www.nuget.org/packages/StardustDL.RazorComponents.Markdown for all versions.

```sh
dotnet add package StardustDL.RazorComponents.Markdown --version <version>
```

> For latest build, use the following source.
> https://sparkshine.pkgs.visualstudio.com/StardustDL/_packaging/feed/nuget/v3/index.json

1. Add static assets to `index.html`.

```html
<link rel="stylesheet" type="text/css" href="_content/StardustDL.RazorComponents.Markdown/highlight.js/github.css">
<link rel="stylesheet" type="text/css" href="_content/StardustDL.RazorComponents.Markdown/katex/katex.min.css">

<script src="_content/StardustDL.RazorComponents.Markdown/component-min.js" type="text/javascript"></script>
<script src="_content/StardustDL.RazorComponents.Markdown/mermaid/mermaid.min.js" type="text/javascript"></script>
```

3. Use the component in Razor components.

```razor
<StardustDL.RazorComponents.Markdown.MarkdownRenderer Value="@MarkdownText" />
```

## Preview

Here are some screenshots from the demo project.

### Header

![](docs/images/demo1.png)

### Code with highlighting

![](docs/images/demo2.png)

### Extensions

![](docs/images/demo3.png)

### Mathematics

![](docs/images/demo4.png)

### Diagram

![](docs/images/demo5.png)

## Dependencies

- [Markdig](https://github.com/lunet-io/markdig)
- [Katex](https://github.com/KaTeX/KaTeX)
- [Mermaid.js](https://github.com/mermaid-js/mermaid)
- [Highlight.js](https://github.com/highlightjs/highlight.js)

## License

Apache-2.0