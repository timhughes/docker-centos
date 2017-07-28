
FROM timhughes/centos:centos6_buildpack-deps
RUN git clone https://github.com/sstephenson/ruby-build.git
WORKDIR ruby-build
RUN ./install.sh
RUN curl -fsSL https://github.com/sstephenson/ruby-build/raw/c636d214f79900d30b8b2e9b6d49891db9ebf068/share/ruby-build/patches/changeset_r41808-187.diff | CFLAGS="-O2 -fno-tree-dce -fno-optimize-sibling-calls"  ruby-build --patch 1.8.7-p374  /usr/local/ruby
ENV PATH /usr/local/ruby/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
RUN gem install --no-ri --no-rdoc bundler
