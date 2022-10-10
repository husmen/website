# HUSMEN | Personal Website
Made by Hugo:
- Go v1.19.2
- Hugo Extended v0.104.3
- Academic Theme v5.7.0
## Address
[https://husmen.xyz](https://husmen.xyz)
## Static Files
[https://github.com/husmen/husmen.github.io/](https://github.com/husmen/husmen.github.io/)

# Getting started with the same template

```bash
choco install go hugo-extended
hugo new site website
cd website
git init
git submodule add https://github.com/wowchemy/starter-hugo-academic themes/academic
hugo mod init github.com/husmen/website
```
Add following lines to `config.toml`
```toml
theme = 'academic'
ignoreErrors = ["error-remote-getcsv"]

[module]
[[module.imports]]
  path = 'github.com/wowchemy/wowchemy-hugo-themes/modules/wowchemy/v5'

```
```bash
hugo mod get github.com/wowchemy/wowchemy-hugo-themes/modules/wowchemy/v5@v5.7.1-0.20221002163318-39a618761acc
hugo server -D
```

```
hugo new posts/my-first-post.md
```

```
---
title: "My First Post"
date: 2019-03-26T08:47:11+01:00
draft: true
---
```

```yaml
security:
  funcs:
    getenv:
      - ^HUGO_
      - ^WC_
```

- https://github.com/wowchemy/wowchemy-hugo-themes/discussions/2559#discussioncomment-1840591