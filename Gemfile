source "https://rubygems.org"

# # Specifichiamo la versione di Ruby richiesta
# ruby "~> 3.3.0"

# La gemma principale per GitHub Pages
gem "github-pages", "~> 232"

# Specifichiamo alcune dipendenze chiave con le loro versioni esatte
gem "jekyll", "~> 3.10.0"
gem "nokogiri", "~> 1.16.7"
gem "kramdown", "~> 2.4.0"
gem "kramdown-parser-gfm", "~> 1.1.0"

# Gemme di supporto per vari sistemi operativi
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.17.0"
  gem "jekyll-seo-tag", "~> 2.8.0"
  # Aggiungi qui altri plugin che ti servono dalla lista
end

gem "minima", "~> 2.5"
gem "chulapa-jekyll"

# Gemme necessarie per Windows
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance-booster per watching directories su Windows
gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]

# Lock http_parser.rb per JRuby
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]