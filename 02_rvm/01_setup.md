!SLIDE smbullets incremental transition=zoom
### RVM is Ruby enVironment (version) Manager ###

  * You can install it in several ways:
  * Simple copy &amp; paste bash command
  * As a Ruby gem
  * From Git source

!SLIDE code transition=uncover
## Installing RVM ##

    @@@sh
    $ bash < <(curl -s https://rvm.beginrescueend.com/install/rvm)

Update your .bash\_profile to load RVM:

    @@@sh
    # RVM
    if [[ -s /Users/steven/.rvm/scripts/rvm ]] ; then
      source /Users/steven/.rvm/scripts/rvm ;
    fi
  
<div class="footer">
  Facilitated by: Booz, Allen, Hamilton | Presented by: <a href="http://twitter.com/stevenhaddox">@stevenhaddox</a>
</div>

!SLIDE code transition=uncover
## Installing Rubies ##

    @@@sh
    # List available rubies:
    $ rvm list known
    # List currently installed rubies:
    $ rvm list
    # Install any available ruby:
    $ rvm install ruby-1.9.2
    $ rvm install jruby-1.6.0
    $ rvm install macruby
    $ rvm install rbx

<div class="footer">
  Facilitated by: Booz, Allen, Hamilton
</div>


!SLIDE code transition=uncover
## Installing Packages ##

If you want to use RVM in production without sudo you'll want your own packages, RVM gives you that too :)

    @@@sh
    # List packages available
    $ rvm package help
    $ rvm package install ree_dependencies
    $ rvm install ree --with-readline-dir=$rvm_usr_path --with-iconv-dir=$rvm_usr_path --with-zlib-dir=$rvm_usr_path --with-openssl-dir=$rvm_usr_path

<div class="footer">
  Facilitated by: Booz, Allen, Hamilton
</div>


!SLIDE smbullets incremental transition=uncover
## Gemsets ##

  * RVM provides you with "gemsets" which allow you to:
  * Install gems on a per-project basis avoiding conflicts
  * Migrate / test different Rubies easily

!SLIDE code transition=uncover
## Using Gemsets ##

    @@@sh
    # Create a gemset
    $ rvm gemset create mygemset
    # Use the gemset
    $ rvm gemset use mygemset

