# Container for the PyleoclimPaper notebooks (v1.0.0)

The `.binder/Dockerfile` at the root of this repo pulls a prebuilt image from
Quay so that myBinder does not need to solve the environment:

    docker pull quay.io/linkedearth/pyleoclimpaper:v1.0.0

Published digest: `sha256:cd3db840540ba5e9f5df94723a0ad258dfc9bfc175e662734ace643f660b5c78`

## Files

- `environment.yml`: pinned top-level packages (latest releases as of 2024-07-24,
  when the notebooks were last updated; Pyleoclim 1.1.0, pylipd @ 0f7743afac).
- `environment.lock.yml`, `pip.lock.txt`: the full set of packages actually
  installed in the published image (exported at build time).
- `Dockerfile`: builds on `quay.io/jupyter/minimal-notebook:x86_64-2024-07-22`.

## Rebuilding

    docker build --platform linux/amd64 -t quay.io/linkedearth/pyleoclimpaper:v1.0.0 docker/
    docker push quay.io/linkedearth/pyleoclimpaper:v1.0.0
