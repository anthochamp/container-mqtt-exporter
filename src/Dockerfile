# 1.6.1 introduces a memory leak ?
FROM kpetrem/mqtt-exporter:1.6.1@sha256:e105467fe086f9b01de7da6aa25acf135d9262a270d35c3895dc813c154ddb22

COPY --chmod=775 /rootfs/docker-entrypoint.sh /

ENTRYPOINT [ "/docker-entrypoint.sh" ]
CMD [ "python", "/opt/mqtt-exporter/exporter.py" ]
