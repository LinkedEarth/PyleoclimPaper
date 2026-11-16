# Jupyter docker-stacks image from 2024-07-22 (amd64): already Binder-compatible
# (user jovyan, uid 1000, Jupyter server installed).
FROM quay.io/jupyter/minimal-notebook:x86_64-2024-07-22

COPY --chown=${NB_UID}:${NB_GID} environment.yml /tmp/environment.yml
RUN mamba env update -n base -f /tmp/environment.yml && \
    mamba clean --all -f -y && \
    mamba env export -n base > /opt/conda/environment.lock.yml && \
    pip freeze > /opt/conda/pip.lock.txt && \
    fix-permissions "${CONDA_DIR}" && fix-permissions "/home/${NB_USER}"

LABEL org.opencontainers.image.source="https://github.com/LinkedEarth/PyleoclimPaper" \
      org.opencontainers.image.description="Environment for PyleoclimPaper v1.0.0 notebooks (Pyleoclim 1.1.0)"
