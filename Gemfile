source "https://rubygems.org"

# Jekyll 4, built by GitHub Actions (.github/workflows/pages.yml) rather than the older
# github-pages gem, which is stuck on Jekyll 3.
gem "jekyll", "~> 4.4"

# `jekyll serve` needs a web server, which Ruby stopped bundling in 3.0.
gem "webrick", "~> 1.8"

# Windows has no zoneinfo database of its own.
platforms :windows do
  gem "tzinfo-data"
  gem "wdm", ">= 0.2"
end
