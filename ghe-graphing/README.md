# collectd

```
docker build -t ghe-collectd .
docker run -it -p 25826:25826/udp --link graphite --rm --name ghe-collectd ghe-clooectd
```


# graphite

```
docker run -d --name graphite --restart=always -p 80:80 -p 2003-2004:2003-2004 -p 2023-2024:2023-2024 -p 8125:8125/udp -p 8126:8126 graphiteapp/graphite-statsd
```

# grafana

```
docker run -d --name grafana -p 3000:3000 grafana/grafana
```