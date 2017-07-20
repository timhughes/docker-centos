FROM timhughes/centos:centos6_buildpack-deps
RUN git clone https://github.com/sstephenson/ruby-build.git
WORKDIR ruby-build
RUN ./install.sh
RUN  ruby-build 2.1.8 /usr/local/ruby
ENV PATH /usr/local/ruby/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
RUN gem install bundler

