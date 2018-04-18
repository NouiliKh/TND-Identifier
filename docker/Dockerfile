FROM tensorflow/tensorflow

LABEL maintainer="Zied Guesmi <guesmy.zied@google.com>"

RUN apt-get update && apt-get install -y \
        python3-pip \
        && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

RUN pip3 -no-cache-dir install \
    opencv-python \
    sklearn \
    numpy

COPY ../src /app/src

WORKDIR /app/src

ENTRYPOINT ["python3", "predict.py"]
