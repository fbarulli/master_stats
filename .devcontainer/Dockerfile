
FROM ://mcr.microsoft.com


RUN curl -L https://github.com -o miniforge.sh \
    && bash miniforge.sh -b -p /opt/conda \
    && rm miniforge.sh


ENV PATH="/opt/conda/bin:$PATH"


RUN mamba install -y ipykernel ipython pandas numpy matplotlib
