FROM almalinux:9
#CMD ["ping","google.com"]
RUN dnf install git -y
RUN useradd mahalakshmi

USER mahalakshmi
CMD ["google.com"]
ENTRYPOINT ["ping"]
#docker build -t user:v1 --no-cache -progress=plain .