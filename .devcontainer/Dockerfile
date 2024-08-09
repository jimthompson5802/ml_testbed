FROM continuumio/miniconda3

# Create a conda environment
RUN conda create --name myenv python=3.10

# Activate the conda environment and install pip packages
RUN echo "source activate myenv" > ~/.bashrc
ENV PATH /opt/conda/envs/myenv/bin:$PATH

RUN pip install numpy scipy matplotlib ipython jupyter pandas sympy nose \
    scikit-learn pylint ipykernel black flake8 flake8-pyproject isort pytest