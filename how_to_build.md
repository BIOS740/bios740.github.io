### Install Jeckyll

To install Jekyll, follow the official installation guide at [https://jekyllrb.com/docs/installation/](https://jekyllrb.com/docs/installation/).

Don't use mac's pre-installed ruby, it is outdated. follow the instructions to install a newer version using a version manager like `rbenv` or `rvm`.

### Use as a Ruby Gem

Alternatively, you can install the theme as a Ruby Gem, without creating a new site.

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem "just-the-docs"
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: just-the-docs
```

And then install all relevant dependencies:

```shell
$ bundle
```

To test your theme, run `bundle exec jekyll serve` and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme. Add pages, documents, data, etc. like normal to test your theme's contents.