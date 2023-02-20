FROM telegraf

COPY telegraf.conf /etc/telegraf
COPY entrypoint.sh /

ENTRYPOINT ["/bin/bash", "/entrypoint.sh"]

CMD ["telegraf"]

# docker run --rm -v ${PWD}:/src telegraf:1.19 cp /etc/telegraf.conf /src/example.conf
# docker run --rm telegraph:1.19 telegraph config telegraf.conf
# docker run -t telegraph:1.19 telegraph config | egrep -v '(^ *^M$|^ *#)'