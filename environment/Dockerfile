# hash:sha256:a91af2500f57e6ad904d196bab01e0e2d3e8c61e04a765b1fa61e30ab2228be4
FROM registry.codeocean.com/codeocean/miniconda3:4.12.0-python3.9-ubuntu20.04

ARG DEBIAN_FRONTEND=noninteractive

RUN conda install -y --channel=conda-forge \
        numpy==1.23.5 \
        pandas==1.2.5 \
        pytorch==1.12.1 \
        scipy==1.8.1 \
        tensorflow==2.4.1 \
    && conda clean -ya

RUN pip install -U --no-cache-dir \
    jupyter==1.0.0 \
    scikit-learn==1.3.0 \
    torch-cluster==1.6.1 \
    torch-geometric==2.3.1 \
    torch-geometric-temporal==0.54.0 \
    torch-scatter==2.1.1 \
    torch-sparse==0.6.17 \
    torch-spline-conv==1.2.2
