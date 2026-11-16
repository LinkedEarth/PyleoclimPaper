# myBinder pulls this prebuilt image instead of solving the environment.
# The image is built from docker/ in this repo; see docker/README.md.
# The digest pins the exact image even if the v1.0.0 tag is ever overwritten.
FROM quay.io/linkedearth/pyleoclimpaper:v1.0.0@sha256:cd3db840540ba5e9f5df94723a0ad258dfc9bfc175e662734ace643f660b5c78

# Set working directory
WORKDIR /home/jovyan

# Copy repository files into the container
COPY . /home/jovyan/

# Set the default command to start Jupyter
CMD ["jupyter", "lab", "--ip=0.0.0.0", "--port=8888", "--no-browser"]