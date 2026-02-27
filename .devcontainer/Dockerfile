# Use the official Microsoft Python base (stable & fast)
FROM ://mcr.microsoft.com

# Install Miniforge (the best Conda/Mamba alternative for Codespaces)
RUN curl -L https://github.com -o miniforge.sh \
    && bash miniforge.sh -b -p /opt/conda \
    && rm miniforge.sh

# Add conda to the system path
ENV PATH="/opt/conda/bin:$PATH"

# Pre-install the kernel so Jupyter works immediately
RUN mamba install -y ipykernel ipython pandas numpy matplotlib
