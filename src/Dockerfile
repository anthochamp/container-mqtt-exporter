# 1.6.1 introduces a memory leak ?
FROM kpetrem/mqtt-exporter:1.8.1@sha256:f3aecdb53d0252ed153ea8472614d9bbc31d56ae2fc5e5d0ef59667bc4c248c8

COPY --chmod=775 /rootfs/docker-entrypoint.sh /

ENTRYPOINT [ "/docker-entrypoint.sh" ]
CMD [ "python", "/opt/mqtt-exporter/exporter.py" ]
