FROM graphframes/dev

RUN apt-get update && \
    apt-get install -y ruby ruby-dev python3-pip && \
    apt-get clean

RUN pip install sphinx==1.8 numpy
RUN gem install jekyll bundler jekyll-redirect-from
RUN pip install jinja2==2.11.3 markupsafe==2.0

WORKDIR /mnt/graphframes

# redefine the entrypoint to empty so that we can run the shell command with `docker run`.
ENTRYPOINT []

