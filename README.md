# feditext.github.io

[Jekyll](https://jekyllrb.com) project for https://www.feditext.com

# local testing on macOS with Homebrew, without Docker

```
# from Jekyll's macOS installation instructions
brew install chruby ruby-install xz
ruby-install ruby 3.1.3
echo "source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh" >> ~/.zshrc # or ~/.bash_profile or fish or...
echo "source $(brew --prefix)/opt/chruby/share/chruby/auto.sh" >> ~/.zshrc
echo "chruby ruby-3.1.3" >> ~/.zshrc # run 'chruby' to see actual version
```

exit and restart your shell

```
ruby -v # should show ruby 3.1.3p185 or newer
bundle install
bundle exec jekyll serve
```

check http://127.0.0.1:4000/
