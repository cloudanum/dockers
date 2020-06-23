ARG BASE_CONTAINER=cloudanum/base_minimal_scipy
FROM $BASE_CONTAINER

LABEL maintainer="Cloudanum"

# Install Tensorflow
RUN pip install --quiet \
    'tensorflow==2.0.0' && \
    fix-permissions $CONDA_DIR && \
    fix-permissions /home/$NB_USER
