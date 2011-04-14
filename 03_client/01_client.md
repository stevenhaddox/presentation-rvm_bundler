!SLIDE smbullets transition=zoom
## RVM::FW Client Configuration##

Pointing RVM to use RVM::FW is the easiest part:

    @@@sh
    $ wget http://<your-server-url>:<port>/db -O ~/.rvm/config/user
    $ rvm reload

Once you have done this RVM will automatically install Rubies from RVM::FW when they are provided!

<div class="footer">
  Facilitated by: Booz, Allen, Hamilton | Presented by: <a href="http://twitter.com/stevenhaddox">@stevenhaddox</a>
</div>