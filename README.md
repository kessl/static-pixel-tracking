# Tracking pixel with GoAccess and Nginx

GoAccess analytics pixel setup with Nginx. [Full writeup here.](https://blog.bitgate.cz/static-site-analytics-with-nginx-goaccess-no-js/). To run on Raspberry Pi, check out [this branch](https://github.com/kessl/static-pixel-tracking/tree/rpi).

- replace `t.bitgate.cz` with your domain name
- obtain initial certificate: `sudo ./init-letsencrypt.sh`
- run `docker-compose up`
- go to `http://localhost/cat.gif?u=some-url`
- watch real time report at `http://localhost:7891`
