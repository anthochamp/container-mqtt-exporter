# 1.6.1 introduces a memory leak ?
FROM kpetrem/mqtt-exporter:1.6.0

COPY --chmod=775 /rootfs/docker-entrypoint.sh /

ENTRYPOINT [ "/docker-entrypoint.sh" ]
CMD [ "python", "/opt/mqtt-exporter/exporter.py" ]
