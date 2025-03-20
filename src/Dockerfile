# 1.6.1 introduces a memory leak ?
FROM kpetrem/mqtt-exporter:1.7.2@sha256:7e2a27e3dce10427ae46490ede2f74fb7799e9e909baae6f8642fb4d5794f1e0

COPY --chmod=775 /rootfs/docker-entrypoint.sh /

ENTRYPOINT [ "/docker-entrypoint.sh" ]
CMD [ "python", "/opt/mqtt-exporter/exporter.py" ]
