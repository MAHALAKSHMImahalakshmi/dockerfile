FROM almalinux:9
#CMD ["ping","google.com"]
CMD ["google.com"]
ENTRYPOINT ["ping"]
# CMD instruction can be overriden
# We can't override ENTRYPOINT, if we try to do it will override
# We can use combination of CMD and ENTRYPOINT for better results, ENTRYPOINT will have command, default args can be supplied by CMD
# You can always override default args through command line
# ping google.com ping facebook.com