FROM debian

RUN apt-get update && \
	apt-get upgrade -y && \
	apt-get install -y vim gcc

ENTRYPOINT vim

# docker build -t csys .
# docker run --rm -it csys