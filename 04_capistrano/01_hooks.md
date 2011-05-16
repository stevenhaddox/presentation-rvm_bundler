!SLIDE transition=zoom
## Capistrano ##

Once your project is setup using RVM and/or Bundler you can easily integrate these tools into your deployment strategies.

<div class="footer">
  Facilitated by: Booz, Allen, Hamilton | Presented by: <a href="http://twitter.com/stevenhaddox">@stevenhaddox</a>
</div>

!SLIDE code transition=uncover
## Bundler ##

Symlink vendor/bundle to shared/vendor_bundle  
Add the following line to your config/deploy.rb file:
  
    @@@Ruby
    require "bundler/capistrano"

<div class="footer">
  Facilitated by: Booz, Allen, Hamilton | Presented by: <a href="http://twitter.com/stevenhaddox">@stevenhaddox</a>
</div>

!SLIDE code transition=uncover
## RVM ##

Add the following to your config/deploy.rb file:

    @@@Ruby
    # Add RVM's lib directory to the load path.
    $:.unshift(File.expand_path('./lib', ENV['rvm_path']))
    require "rvm/capistrano"            # Load RVM's capistrano plugin.
    set :rvm_ruby_string, 'ree@rails3'  # Load env you want it to run in.

<div class="footer">
  Facilitated by: Booz, Allen, Hamilton | Presented by: <a href="http://twitter.com/stevenhaddox">@stevenhaddox</a>
</div>