# 1.6.1 introduces a memory leak ?
FROM kpetrem/mqtt-exporter:1.9.0@sha256:c9b5074f23daadbbe2fdf008e440378cd4cffac024bcedf2d1c8f29ddaa9ab5c

COPY --chmod=775 /rootfs/docker-entrypoint.sh /

ENTRYPOINT [ "/docker-entrypoint.sh" ]
CMD [ "python", "/opt/mqtt-exporter/exporter.py" ]
