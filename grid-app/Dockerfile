FROM ricklamers/gridstudio:release as base

RUN rm -rf /home/source
# copy over all files to /home/source/
WORKDIR /home/source/
COPY . /home/source/

# expose ports
EXPOSE 8080
EXPOSE 4430

WORKDIR /home/source/proxy/

CMD ["bash","run-manager-proxy.sh"]