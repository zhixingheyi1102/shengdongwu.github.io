source 'https://rubygems.org'

# 使用 github-pages gem，它会指定正确的 Jekyll 版本和插件
gem 'github-pages', group: :jekyll_plugins
gem 'webrick', '~> 1.8'
gem 'tzinfo-data'
gem 'wdm', '>= 0.1.0' if Gem.win_platform?

# 以下插件需要与 _config.yml 的 plugins 部分匹配
# 不要指定版本，让 github-pages 管理版本
group :jekyll_plugins do
  gem 'jekyll-feed'
  gem 'jekyll-gist'
  gem 'jekyll-paginate'
  gem 'jekyll-sitemap'
  gem 'jekyll-redirect-from'
  gem 'jemoji'
  gem 'breakpoint'
  gem 'faraday-retry'
end
