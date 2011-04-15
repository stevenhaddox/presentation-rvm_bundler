!SLIDE smbullets transition=zoom
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