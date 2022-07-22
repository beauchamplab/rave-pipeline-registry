# Compile locally

The development of this website is under OSX. I haven't tested other operating systems. The compilation require `brew` and `npm`. Please install them first.

To set up environment, please `cd` to the project directory and run the following command line-by-line

```sh
brew install ruby
export PATH="$HOMEBREW_PREFIX/opt/ruby/bin:$PATH"
gem install bundler
bundle config path vendor/bundle
bundle install --jobs 4 --retry 3
```

To launch the local server,

```sh
export PATH="$HOMEBREW_PREFIX/opt/ruby/bin:$PATH"
bundle exec jekyll serve
```