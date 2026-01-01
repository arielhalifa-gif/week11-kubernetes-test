the dockerfile is the explanation for docker to build the image

FROM  # the app to use for the app

WORKDIR # the directory that the app will be store in the container

COPY requirements.txt # for better cache first copy only the requirements

RUN pip install... # install the requirements so the app can run without chache

COPY . . # copy the rest of the app