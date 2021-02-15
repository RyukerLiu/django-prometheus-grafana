# Django Prometheus Grafana

Docker-composed django, prometheus and grafana services

```
docker-compose up
```

## Grafana

http://localhost:3000/

Default admin user is admin/admin.

https://hub.docker.com/r/grafana/grafana

https://www.sipios.com/blog-tech/monitoring

In config add data source with prometheus type: http://prometheus:9090

Then, you could create the dashboard with metrics you like

## Prometheus

http://localhost:9090/graph

http://localhost:9090/graph?g0.range_input=1h&g0.stacked=1&g0.expr=django_http_requests_total_by_method_total&g0.tab=0

https://docs.timescale.com/latest/tutorials/tutorial-howto-monitor-django-prometheus

https://github.com/korfuri/django-prometheus
