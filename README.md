# Wisdom

Wisdom is a fast, minimalist, monospace theme for [Hugo](https://gohugo.io/).\
If you like it [give us a :star:](https://github.com/maxrodrigo/hugo-theme-wisdom)!

### Features

- Dark and Light Color Schemes
- Color-Scheme Preference Aware
- SEO Friendly
- Keywords
- Multilingual and i18n support
- Comments support
- Production environment aware
- Twitter Cards
- OpenGraph
- Google Analytics
- Custom CSS and JS support
- CallOuts
- Taxonomies

## 1. Install

### 1.1 As a Git Submodule

The theme will be added as a dependency to the original repository. When using CI tools like Netlify, Jenkins etc., the submodule method is required.

1. Inside your Hugo site directory, run:

    ```sh
    git submodule add https://github.com/maxrodrigo/hugo-theme-wisdom themes/wisdom
    ```

2. Set the theme into the configuration file:

    ```yaml
    # config.yaml
    theme: "wisdom"
    ```

    ```toml
    # config.toml
    theme = "wisdom"
    ```

For more information read the official [quick start guide](https://gohugo.io/getting-started/quick-start/) of Hugo.

## 2. Getting Started

### 2.1 Example Configuration

See [configuration example](exampleSite/config.toml).

### 2.2 Add Menu

To add a menu, add a menu section to your site's config.toml:

```toml
[menu]
[[menu.main]]
  identifier = 'home'
  name = 'home'
  url = '/'
  weight = -110
[[menu.main]]
  identifier = 'posts'
  name = 'posts'
  url = '/posts/'
  weight = -100
```
### 2.3 Favicon

You can set the favicon by placing `favicon.ico` in the `static` directory.

```
- content
- static
  └── favicon.ico
```

### 2.4 Page Configuration

Defaults

```toml
title = "{{ replace .Name "-" " " | title }}"
date = {{ .Date }}
draft = true
noindex = false
```

## Development

Browse `exampleSite` and serve.

```sh
cd exampleSite
hugo serve -t ../..
```

## Contributing

Have you found a bug or got an idea for a new feature? Feel free to use the [issue tracker](https://github.com/maxrodrigo/hugo-theme-wisdom/issues) to let me know. Or make directly a [pull request](https://github.com/maxrodrigo/hugo-theme-wisdom/pulls).

## License

This theme is released under the [MIT license](https://github.com/maxrodrigo/hugo-theme-wisdom/blob/master/LICENSE).
