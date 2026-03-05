# 1.6.1 introduces a memory leak ?
FROM kpetrem/mqtt-exporter:1.11.2@sha256:a756613b9a4c9b386c308354d708af549e8dd115d98df815c58ac09320787e9a

COPY --chmod=775 /rootfs/docker-entrypoint.sh /

ENTRYPOINT [ "/docker-entrypoint.sh" ]
CMD [ "python", "/opt/mqtt-exporter/exporter.py" ]
