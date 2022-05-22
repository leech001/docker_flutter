FROM ubuntu:rolling

ENV LANG en_US.utf8
ENV PATH="${PATH}:/flutter/bin"

#Update Ubuntu and clean
RUN apt-get update && apt-get dist-upgrade -y && apt-get autoremove && apt-get autoremove
RUN apt-get install -y cmake ninja-build clang build-essential pkg-config libgtk-3-dev liblzma-dev lcov curl zip unzip git

# Add for packet system_tray (https://pub.dev/packages/system_tray)
# RUN apt-get install -y libappindicator3-dev gir1.2-appindicator3-0.1

# install Flutter branch master
RUN git clone https://github.com/flutter/flutter.git

# Enable flutter linux desktop
RUN flutter config --enable-linux-desktop

SHELL [ "/bin/bash", "-c" ]
CMD [ "flutter", "doctor" ]
