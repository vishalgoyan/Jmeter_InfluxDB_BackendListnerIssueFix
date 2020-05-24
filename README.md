# Jmeter_InfluxDB_BackendListnerIssueFix

Jmeter, by default adds the sampler metrics for a common sampler in the span of influxDB interval duration and send aggregated values to Influx DB after givenn interval.
This causes the discrepencies between Influx DB metrics and Jmeter Metrics.

To resolve this issue, I have modified Jmeter source code and changed the default influxDB send interval to 1 second.
