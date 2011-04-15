!SLIDE smbullets transition=zoom
## RVM::FW Client Configuration##

Installing RVM if it isn't installed yet:

    @@@sh
    $ bash < <( curl http://<your-server>:<port>/releases/rvm-install-latest )

Configure RVM to use RVM::FW's Rubies:

    @@@sh
    $ wget http://<your-server>:<port>/db -O ~/.rvm/config/user
    $ rvm reload

Once you have done this RVM will automatically install Rubies from RVM::FW when they are provided!

<div class="footer">
  Facilitated by: Booz, Allen, Hamilton | Presented by: <a href="http://twitter.com/stevenhaddox">@stevenhaddox</a>
</div>