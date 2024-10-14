FROM jupyter/tensorflow-notebook:python-3.10
COPY requirements.txt ./requirements.txt
RUN pip install --no-cache-dir -r ./requirements.txt

# Allow drivers installed by the nvidia-driver-installer to be located
ENV LD_LIBRARY_PATH=${LD_LIBRARY_PATH}:/usr/local/nvidia/lib64:/usr/local/nvidia/lib
# Also, utilities like `nvidia-smi` are installed here
ENV PATH=${PATH}:/usr/local/nvidia/bin
