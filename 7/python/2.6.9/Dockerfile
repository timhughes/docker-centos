FROM timhughes/centos:centos7_buildpack-deps
RUN git clone git://github.com/yyuu/pyenv.git /tmp/pyenv
RUN cd /tmp/pyenv/plugins/python-build && sh install.sh
RUN rm -rf /tmp/pyenv
RUN python-build 2.6.9 /usr/local/python
ENV PATH /usr/local/python/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
