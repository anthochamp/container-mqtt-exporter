# 1.6.1 introduces a memory leak ?
FROM kpetrem/mqtt-exporter:1.6.0@sha256:c1ade5ba4ff9cfb51fe36b9d0001bc81abc095b0266ba7cfc4179a9ba7df2d47

COPY --chmod=775 /rootfs/docker-entrypoint.sh /

ENTRYPOINT [ "/docker-entrypoint.sh" ]
CMD [ "python", "/opt/mqtt-exporter/exporter.py" ]
