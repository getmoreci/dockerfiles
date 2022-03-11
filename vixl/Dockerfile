FROM ubuntu:18.04

RUN apt-get update && apt-get install -y \
  clang-4.0 \
  clang-format-4.0 \
  clang-tidy-4.0 \
  g++ \
  scons \
  wget \
  && rm -rf /var/lib/apt/lists/*

RUN wget --no-verbose --output-document /usr/bin/cpplint.py https://raw.githubusercontent.com/google/styleguide/gh-pages/cpplint/cpplint.py
RUN chmod a+x /usr/bin/cpplint.py
