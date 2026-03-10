# MQTT Exporter Container

![GitHub License](https://img.shields.io/github/license/anthochamp/container-mqtt-exporter?style=for-the-badge)
![GitHub Release](https://img.shields.io/github/v/release/anthochamp/container-mqtt-exporter?style=for-the-badge&color=457EC4)
![GitHub Release Date](https://img.shields.io/github/release-date/anthochamp/container-mqtt-exporter?style=for-the-badge&display_date=published_at&color=457EC4)

Container images based on [mqtt-exporter](https://github.com/kpetrem/mqtt-exporter), a generic Prometheus exporter that subscribes to MQTT topics and exposes them as metrics.

## How to use this image

```shell
docker run -p 9114:9114 \
  -e MQTT_ADDRESS=mqtt-broker:1883 \
  anthochamp/mqtt-exporter
```

## Port

| Port | Protocol | Description |
| --- | --- | --- |
| `9114` | TCP | Prometheus metrics endpoint (default) |

## Configuration

This container adds Docker secrets support: append `__FILE` to any environment variable name to read its value from a file (e.g., `MQTT_PASSWORD__FILE=/run/secrets/mqtt_password`).

All environment variables supported by mqtt-exporter are available. Refer to the [mqtt-exporter documentation](https://github.com/kpetrem/mqtt-exporter#configuration) for the full list.

## References

- [mqtt-exporter on GitHub](https://github.com/kpetrem/mqtt-exporter)
- [Prometheus](https://prometheus.io/)
