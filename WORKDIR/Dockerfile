FROM almalinux:9
RUN mkdir /tmp/workdir-demo
#RUN cd /tmp/workdir-demo this will not work error
WORKDIR /tmp/workdir-demo 
RUN pwd
RUN echo "Hello I am in work dir" > hello.txt
CMD ["sleep","1000"]
# workdir
# docker build -t workdir:v1 --no-cache --progress=plain .
# Used cmd can overrideden but not entry point
# •	Each RUN instruction runs in a new shell and a new intermediate container.
# •	Changes such as cd (changing directory) inside a RUN command affect only that single command instance.
# •	When the next RUN command starts, it resets back to the default working directory (usually /).
# So, RUN cd /tmp/workdir-demo changes directory only temporarily and does not persist for subsequent commands.
# Correct way to set working directory:
# Use the WORKDIR instruction instead, which sets the working directory for all subsequent commands (RUN, CMD, ENTRYPOINT, COPY, ADD):
