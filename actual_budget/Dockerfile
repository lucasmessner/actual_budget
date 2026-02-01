ARG BUILD_FROM
FROM $BUILD_FROM

# Install Python for example server
RUN apk add --no-cache python3

# Set working directory to persistent data folder
WORKDIR /data

# Copy the startup script
COPY run.sh /
RUN chmod a+x /run.sh

CMD [ "/run.sh" ]
