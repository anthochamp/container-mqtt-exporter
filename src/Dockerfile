# 1.6.1 introduces a memory leak ?
FROM kpetrem/mqtt-exporter:1.12.1@sha256:dca3255f35310f6ceb80ed1de94eebd1fe9def7aacaec4107fe37cdaa9eb3be0

COPY --chmod=775 /rootfs/docker-entrypoint.sh /

ENTRYPOINT [ "/docker-entrypoint.sh" ]
CMD [ "python", "/opt/mqtt-exporter/exporter.py" ]
