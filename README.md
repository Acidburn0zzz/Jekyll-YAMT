# WORK IN PROGRESS! STILL NEED TO FIX MINOR THINGS AND TO WRITE THE DOCS

# [YAMT - Yet Another Minimal Theme](https://yamt.netlify.app/)
[![Netlify Status](https://api.netlify.com/api/v1/badges/249c3da6-7b23-4b57-915d-71934329e306/deploy-status)](https://yamt.netlify.app/)
![supports mathjax](https://img.shields.io/badge/Supports-MathJAX-blue)
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/PandaSekh/Jekyll-YAMT/issues)
![GitHub forks](https://img.shields.io/github/forks/PandaSekh/Jekyll-YAMT?label=Fork%20it%21&style=social)
## [Live Demo](https://yamt.netlify.app/)
YAMT is a minimal [Jekyll](http://jekyllrb.com) theme focused on simplicity and ease-of-use. It has great modularity, allowing you to easily decide what you actually want on your website.

## Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Customize](#options)
  - [Header](#header)
  - [Post](#post)
- [Development](#development)
- [Credits](#credits)
- [License](#license)

## Features
- Minimal and clean design.
- Fully modular: activate and load only what you really need.
- Works great on mobile and smaller screens.
- Supports [Disqus](https://disqus.com/) comments activated only on button press, if you activate them.
- [Google Analytics](https://www.google.com/analytics/) support.
- [Open Graph](https://ogp.me/) and [Twitter Cards](https://developer.twitter.com/en/docs/tweets/optimize-with-cards/guides/getting-started) support to better index the website content on search engines and social networks.
- [MathJAX](https://www.mathjax.org/) and [LaTeX](https://www.latex-project.org/) optional support. Write beautiful math!
- [RSS](https://github.com/jekyll/jekyll-feed) support.
- Beautiful [Syntax Highlight](https://yamt.netlify.app/2020/05/19/special-formatting.html#syntax-highlight). Write some code and show it in a graceful way.
- 

## Installation
There are four way to use YAMT: Netlify (suggested, as this theme has a contact module built-in working only on Netlify), Github Pages, as a gem-based theme, by forking this repo or by copying all the files into your directory.

### Netlify
1. [Fork this repo](https://github.com/PandaSekh/Jekyll-YAMT/generate). You can copy only master, set it to private or public and name it however you want.
2. Go to [Netlify](https://app.netlify.com/), create a New site from Git, choose your repo or all repos, no difference. Back to Netlify, select the recently forked repo.
3. Owner and branch are good to go. In build command write `bundle exec jekyll build` and publishing directory should be `_site/`.
4. Deploy. Your site will shortly be available. Under domain settings you can change your subdomain, or add a primary level one. 

### Github Pages
Github Pages uses the [--safe flag](https://jekyllrb.com/docs/configuration/options/) to build jekyll websites, which disable custom plugins, caching to disk and ignore symbolic links. Because of that, I suggest you to use any other method. Netlify works great with a 5 minute config, so I suggest you use it.


### Remote theme
1. Have a gemfile with only the following content:

    ```ruby
    source "https://rubygems.org"

    gem "github-pages", group: :jekyll_plugins
    ```

2. Run the following command:

   ```bash
   bundle
   ```

### Gem-based theme 
1. Add this line to your Jekyll site's `Gemfile`:

    ```ruby
    gem "yamt"
    ```

2. And add this line to your Jekyll site's `_config.yml`:

    ```yaml
    theme: yamt
    ```

3. And then execute:

    ``` bash
    $ bundle
    ```

4. Or install it yourself as:
    
    ``` bash
    $ gem install yamt
    ```

## Usage

TODO: Write usage instructions here. Describe your available layouts, includes, sass and/or assets.

## Development

To set up your environment to develop this theme, run `bundle install`.

Your theme is setup just like a normal Jekyll site! To test your theme, run `bundle exec jekyll serve` and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme. Add pages, documents, data, etc. like normal to test your theme's contents. As you make modifications to your theme and to your content, your site will regenerate and you should see the changes in the browser after a refresh, just like normal.

When your theme is released, only the files in `_layouts`, `_includes`, `_sass` and `assets` tracked with Git will be bundled.
To add a custom directory to your theme-gem, please edit the regexp in `yamt.gemspec` accordingly.

## Credits
Inspired by [Lagrange by LeNPaul](https://lenpaul.github.io/Lagrange/).

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
