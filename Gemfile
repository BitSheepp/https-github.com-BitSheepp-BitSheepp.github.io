source "https://rubygems.org"

# 固定 Jekyll 4 系（GitHub 容器默认是 Jekyll 3，不要混用）
gem "jekyll", "~> 4.3.3"
gem "webrick"  # 本地 serve 用

# —— 插件（尽量选择纯 Ruby 插件）——
group :jekyll_plugins do
  gem "jekyll-feed"
  gem "jekyll-sitemap"
  gem "jekyll-seo-tag"
  gem "jemoji"

  # 常用增强
  gem "jekyll-paginate-v2"
  gem "jekyll-toc"
  gem "jekyll-archives-v2"
  gem "jekyll-link-attributes"
  gem "jekyll-regex-replace"
  gem "jekyll-tabs"
  gem "jekyll-scholar"        # 若不需要学术引用，先注释掉
  gem "jekyll-minifier"       # 纯 Ruby 压缩器，替代 terser（JS 压缩会弱些，但更稳）
  # gem "jekyll-terser"       # 如需更强 JS 压缩，后续再加；先跑通为主
  gem "jekyll-twitter-plugin"
end

# 其他 Ruby 依赖（不参与 jekyll 插件加载）
group :other_plugins do
  gem "css_parser"
  gem "feedjira"
  gem "httparty"
  gem "classifier-reborn"
  gem "observer"
  gem "ostruct"
end
