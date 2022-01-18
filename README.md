# Wisdom

A simple yet powerful monospaced theme for [Hugo](https://gohugo.io/).

### Features

- Auto Dark Mode
- SEO Friendly
- Keywords
- Multilingual and i18n support
- Disqus
- Production environment aware
- Twitter Cards
- Opengraph
- Google Analytics

## Install as a git submodule

The theme will be added as a dependency to original repository. When using CI tools like Netlify, Jenkins etc., submodule method is required.

In your Hugo site directory, run:

```sh
git submodule add https://github.com/maxrodrigo/hugo-theme-wisdom themes/wisdom
```

## Install with git clone

In your Hugo site directory, run:

```sh
git clone https://github.com/maxrodrigo/hugo-theme-wisdom themes/wisdom
```

## Configure

Open `config.toml` in the base of the Hugo site and ensure the theme option is set to `wisdom`.

```toml
theme = "wisdom"
```

For more information read the official [quick start guide](https://gohugo.io/getting-started/quick-start/) of Hugo.

## Configuration Example

```toml
baseURL = "https://www.maxrodrigo.com/"
title = "My Awesome Website"
theme = "wisdom"

languageCode = "en-us"
enableRobotsTXT = true

googleAnalytics = 'G-MEASUREMENT_ID'

[params]
  author = Max Rodrigo
  latestPostsLimit = 5
  hideReadingTime = false
  hideAuthor = false
  keywords = ["hugo","theme","SEO"]
```

## Add Menu

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

## Front Matter

Defaults

```toml
title = "{{ replace .Name "-" " " | title }}"
date = {{ .Date }}
draft = true
noindex = false
```

## Contributing

Have you found a bug or got an idea for a new feature? Feel free to use the [issue tracker](https://github.com/maxrodrigo/hugo-theme-wisdom/issues) to let me know. Or make directly a [pull request](https://github.com/maxrodrigo/hugo-theme-wisdom/pulls).

## License

This theme is released under the [MIT license](https://github.com/maxrodrigo/hugo-theme-wisdom/blob/master/LICENSE).
