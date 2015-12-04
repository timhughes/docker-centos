FROM timhughes/centos:7
RUN yum -y install gcc openssl-devel libyaml-devel readline-devel zlib-devel patch curl
RUN git clone https://github.com/sstephenson/ruby-build.git
WORKDIR ruby-build
RUN ./install.sh
RUN  ruby-build 2.1.7 /usr/local/ruby
ENV PATH /usr/local/ruby/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
RUN gem install bundler

