FROM timhughes/centos:centos7_buildpack-deps
RUN git clone git://github.com/yyuu/pyenv.git .pyenv
RUN echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bashrc
RUN echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bashrc
RUN echo 'eval "$(pyenv init -)"' >> ~/.bashrc
RUN source ~/.bashrc
RUN pyenv install 2.6.9
RUN pyenv install 2.7.11
RUN pyenv install 3.5.1
