# Wrapper image for Semgrep.
# Keep this as close to upstream as possible: do not change ENTRYPOINT/CMD unless required.
FROM semgrep/semgrep:1.166.0@sha256:c180f0c93a17b420c0af5006214a29d3c747c5459c732b740191adf657dd0068 AS image

LABEL org.opencontainers.image.title="semgrep-wrapper" \
      org.opencontainers.image.description="Wrapper image around upstream semgrep/semgrep for GitHub CI/CD" \
      org.opencontainers.image.source="https://github.com/msilabben/cnapp-module-4-builder" \
      org.opencontainers.image.vendor="msilabben"

FROM image AS test
RUN semgrep --version

FROM image AS final
