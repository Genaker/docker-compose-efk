FROM fluent/fluentd:latest
MAINTAINER your_name SYA-KE
USER fluent
WORKDIR /home/fluent
ENV PATH /home/fluent/.gem/ruby/2.2.0/bin:$PATH
RUN gem install fluent-plugin-elasticsearch
CMD fluentd -c /fluentd/etc/$FLUENTD_CONF -p /fluentd/plugins $FLUENTD_OPT
