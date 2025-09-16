FROM almalinux:9
ENV COURSE="DevOps" \
    STUDENT="MAHALAKSHMi" 
ARG SKILL="AWS"
# How can you use ARG inside container?
# by reasignning arg variable to env variable
ENV SKILL=$SKILL
RUN echo "Hi, Course is: ${course}, STUDENT: ${STUDENT}, skill is: ${SKILL}"
CMD ["sleep", "1000"]
# ARG is build time variables, they can't be accessed inside container. ENV can be accessed build time and then inside container also
# ARG instruction variables can be overriden
# in an exceptional case ARG can be the first instruction to supply version to base OS in FROM, you cant use that version after FROM instruction