# teafyi

[![crates.io](https://img.shields.io/crates/v/teafyi.svg)](https://crates.io/crates/teafyi)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Tea variety guide with brewing parameters and teaware — API client for [teafyi.com](https://teafyi.com).

> **Try the interactive tools at [teafyi.com](https://teafyi.com)**

## Install

`cargo add teafyi`

## Quick Start

```rust
use teafyi::Client;

#[tokio::main]
async fn main() -> Result<(), Box<dyn std::error::Error>> {
    let client = Client::new();
    let result = client.search("sencha").await?;
    println!("{} results", result.total);
    Ok(())
}
```

## Also Available

| Platform | Package | Link |
|----------|---------|------|
| **Python** | `pip install teafyi` | [PyPI](https://pypi.org/project/teafyi/) |
| **npm** | `npm install teafyi` | [npm](https://www.npmjs.com/package/teafyi) |
| **Go** | `go get github.com/fyipedia/teafyi-go` | [pkg.go.dev](https://pkg.go.dev/github.com/fyipedia/teafyi-go) |
| **Rust** | `cargo add teafyi` | [crates.io](https://crates.io/crates/teafyi) |
| **Ruby** | `gem install teafyi` | [rubygems](https://rubygems.org/gems/teafyi) |

## Embed Widget

Embed [TeaFYI](https://teafyi.com) widgets on any website with [teafyi-embed](https://widget.teafyi.com):

```html
<script src="https://cdn.jsdelivr.net/npm/teafyi-embed@1/dist/embed.min.js"></script>
<div data-teafyi="entity" data-slug="sencha"></div>
```

Zero dependencies · Shadow DOM · 4 themes (light/dark/sepia/auto) · [Widget docs](https://widget.teafyi.com)

## Links

- [TeaFYI](https://teafyi.com) — Main site
- [API Documentation](https://teafyi.com/developers/)
- [OpenAPI Spec](https://teafyi.com/api/openapi.json)
- [Glossary](https://teafyi.com/glossary/)

## License

MIT
