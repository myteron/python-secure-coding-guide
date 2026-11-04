source "https://rubygems.org"

# Use the github-pages gem so local builds match GitHub Pages' build
# environment (same Jekyll version, plugins, and dependencies).
# Pin to a current version; without a floor, the resolver can pick a very old
# release (e.g. v170 -> Jekyll 3.6.2) that breaks on modern Ruby.
gem "github-pages", "~> 232", group: :jekyll_plugins

# Plugins used by the site (also declared in _config.yml).
group :jekyll_plugins do
  gem "jekyll-remote-theme"
  gem "jekyll-feed"
  gem "jekyll-seo-tag"
end

# Windows / WSL file-watching helper (harmless elsewhere).
gem "wdm", "~> 0.1.1", platforms: [:windows]

# Gems removed from Ruby's default set in 3.3/3.4 that Jekyll/kramdown still
# need. Without rexml the build fails with a LoadError on Ruby 3.3+.
gem "rexml"
gem "base64"
gem "bigdecimal"
gem "csv"
