The EdgeRouter X is old but still a great router. You can add Geo filtering by following this guide.

Credits:
https://www.cron.dk/firewalling-by-country-on-edgerouter/
https://www.youtube.com/watch?v=Qn5hbdijYJM&t=3s

These guides were a bit old.

I carried this out version: EdgeRouter X v2.0.9-hotfix.7

Create a firewall group:


configure
set firewall group network-group countries_allowed description 'Allowed countries'
set firewall group network-group countries_allowed network 10.254.254.254/31
commit
save

Create the script under
See file country-load
