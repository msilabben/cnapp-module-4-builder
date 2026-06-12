# Wrapper image for Conftest.
# Keep this as close to upstream as possible: do not change ENTRYPOINT/CMD unless required.
FROM openpolicyagent/conftest:v0.68.2@sha256:5fd81e332d7e4bc01daf3ef35371800a9a9720a30c0c37a78de0c5fbe4b6d622 AS image

LABEL org.opencontainers.image.title="conftest-wrapper" \
      org.opencontainers.image.description="Wrapper image around upstream openpolicyagent/conftest for GitHub CI/CD" \
      org.opencontainers.image.source="https://github.com/msilabben/cnapp-module-4-builder" \
      org.opencontainers.image.vendor="msilabben"

FROM image AS test
RUN conftest --version

FROM image AS final
