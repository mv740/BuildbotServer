FROM buildbot/buildbot-master:master

# docker commands
RUN pip install docker-py

#required for lz4
RUN apk add --no-cache gcc python-dev musl-dev

# compression library
RUN pip install lz4

# Add master config file to appropriate directoy
COPY /master/* /var/lib/buildbot/