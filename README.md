# deployment
How to deploy a flask app using caddy &amp; waitress

Getting a flask application deployed so that it stays up and working can be a little tricky. It involves a bit of sysadmin work that is outside of the usual basic skillset of many developers earlier in their career. Thie repo contains an example simple flask app, in the assignment folder, and a set of scripts for installing and setting up first caddy, then waitress. Caddy works as a reverse proxy, listening on port 80 for incoming public web traffic. All incomiing requests are then proxied to our flask app, served by waitress, on port 5000, internally to our server. Both Caddy and Waitress are set up to be managed by systemd and to restart automatically if they fail or if the server reboots.


