# Wrapper image for Trivy.
# Keep this as close to upstream as possible: do not bake vulnerability DBs into the image by default.
FROM aquasec/trivy:0.71.1@sha256:53570e6911c2361ebe7995228088cf83a6b9b73e7f3cdca44bd8f8f425e80fa7 AS image

LABEL org.opencontainers.image.title="trivy-wrapper" \
      org.opencontainers.image.description="Wrapper image around upstream aquasec/trivy for GitHub CI/CD" \
      org.opencontainers.image.source="https://github.com/msilabben/cnapp-module-4-builder" \
      org.opencontainers.image.vendor="msilabben"

FROM image AS test
RUN trivy --version

FROM image AS final
