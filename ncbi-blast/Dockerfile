FROM continuumio/miniconda:4.7.10
MAINTAINER <resl.philipp@bio.lmu.de>

ENV PATH /opt/conda/bin:$PATH

RUN conda config --append channels bioconda && \
	conda config --append channels conda-forge && \
	conda config --append channels anaconda && \
	conda install -c bioconda blast=2.9.0 && \
	conda clean -a -y

CMD ["blastn", "-version"]