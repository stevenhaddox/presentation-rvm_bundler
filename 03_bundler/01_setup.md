!SLIDE code transition=zoom
## Bundler ##

Install the Bundler gem:

    @@@sh
    $ rvm use 1.9.2@mynewapp
    $ gem install bundler

Create your Gemfile:

    @@@Ruby
    source "http://rubygems.org"

    gem "rails", "3.0.5"
    gem "rack-cache"
    gem "nokogiri", "~> 1.4.2"
    gem "capistrano", ">2.0"

<div class="footer">
  Facilitated by: Booz, Allen, Hamilton | Presented by: <a href="http://twitter.com/stevenhaddox">@stevenhaddox</a>
</div>

!SLIDE code transition=uncover
## Bundler Gem Groups ##

You can group your gems by environment:

    @@@Ruby
    source "http://rubygems.org"

    group :production do
      gem "rails", "3.0.5"
      gem "rack-cache"
      gem "nokogiri", "~> 1.4.2"
      gem "pg"
    end

    group :development do
      gem "sqlite3-ruby"
      gem "capistrano", ">2.0"
    end

    group :test do
      gem "rspec-rails"
      gem "cucumber-rails"
    end


<div class="footer">
  Facilitated by: Booz, Allen, Hamilton | Presented by: <a href="http://twitter.com/stevenhaddox">@stevenhaddox</a>
</div>