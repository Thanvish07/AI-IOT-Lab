# Gemfile (FINAL, CLEAN VERSION)

source "https://rubygems.org"

# CRITICAL FIX: Explicitly list the theme gem for GitHub Actions to install
gem "minimal-mistakes-jekyll" 

# We do NOT use the github-pages gem since we are using Actions 
# and explicitly listing all dependencies.

# List necessary plugins:
group :jekyll_plugins do
  gem "jekyll-include-cache"
  gem "jekyll-feed"
  gem "jekyll-sitemap"
  # You can remove others like jekyll-gist, jemoji if not strictly needed, 
  # but they are often included in the MM starter kit.
end

# Windows-only dependency (keep for local testing on Windows)
gem "wdm", "~> 0.1.0" if Gem.win_platform?
