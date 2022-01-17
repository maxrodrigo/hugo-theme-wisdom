# Wisdom

A simple yet powerful monospaced theme for [Hugo](https://gohugo.io/).

### Features

- Auto Dark Mode
- SEO Friendly
- Multilingual Mode
- Disqus

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
title = "Max Rodrigo"

theme = "hugo-theme-wisdom"

languageCode = "en-us"
enableRobotsTXT = true

# Default Params
[Params]
  author =
  latestPostsLimit = 5
  hideReadingTime = false
  hideAuthor = false

[menu]
[[menu.main]]
  identifier = 'home'
  name = '~/'
  url = '/'
  weight = -110
[[menu.main]]
  identifier = 'posts'
  name = 'posts'
  url = '/posts/'
  weight = -100
```


## Contributing

Have you found a bug or got an idea for a new feature? Feel free to use the [issue tracker](https://github.com/maxrodrigo/hugo-theme-wisdom/issues) to let me know. Or make directly a [pull request](https://github.com/maxrodrigo/hugo-theme-wisdom/pulls).

## License

This theme is released under the [MIT license](https://github.com/maxrodrigo/hugo-theme-wisdom/blob/master/LICENSE).
