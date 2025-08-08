
ARG version
FROM almalinux:${version:-9}
ENV COURSE="DevOps" \
    DURATION="100HRS" 
ARG INSTRUCTOR="DevenderReddyMusukula"
ENV INSTRUCTOR=$INSTRUCTOR
RUN echo "Hi, Course is: ${COURSE}, duration is:${DURATION}, instructor is:${INSTRUCTOR}"
CMD ["sleep", "1000"]