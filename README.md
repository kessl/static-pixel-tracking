# Tracking pixel with GoAccess and Nginx

GoAccess analytics pixel setup with Nginx. See the [full writeup](https://blog.bitgate.cz/static-site-analytics-with-nginx-goaccess-no-js/). This setup is intended for Raspberry Pi. To run on different architecture, change docker images in `docker-compose.yml`

- replace `t.bitgate.cz` with your domain name in `nginx.conf`
- update domain name and e-mail address in `init-letsencrypt.sh`
- obtain initial certificate: `sudo ./init-letsencrypt.sh`
- run `docker-compose up`
- go to `http://localhost/cat.gif?u=some-url`
- watch real time report at `http://localhost:7891`
