# Pluralsight-Otel-Infrastructure

Repository containing the infrastructure configuration for my Pluralsight course [Observability with OpenTelemetry and Grafana](http://www.pluralsight.com/courses/opentelemetry-grafana-observability).

It consists out of a docker compose file setting up an observability environment with following elements:
- Blackbox : for probing endpoints
- Prometheus : collecting metrics of the Blackbox probes
- Loki : logging aggregator for all logs generated by the .NET projects
- Tempo : span and trace aggregator generated by the .NET projects
- Grafana : used for all overviews through dashboards
- RabbitMQ : as message queue for distributed message handling between the .NET projects

The .NET projects can be found here [Pluralsight OTEL backend](https://github.com/Depechie/Pluralsight-Otel-Backend).
