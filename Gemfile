# Gemfile

source "https://rubygems.org"

# Use the official GitHub Pages gem to pull in all supported dependencies
gem "github-pages", group: :jekyll_plugins

# Explicitly list jekyll-include-cache for Minimal Mistakes
group :jekyll_plugins do
  gem "jekyll-include-cache"
  gem "jekyll-feed"
  gem "jekyll-sitemap"
end

# Windows-only dependency (keep for local testing on Windows)
gem "wdm", "~> 0.1.0" if Gem.win_platform?
