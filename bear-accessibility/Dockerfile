FROM python:3.6
RUN apt update
RUN DEBIAN_FRONTEND=noninteractive apt install -y npm libx11-xcb1 libxcomposite1 libxcursor1 libxss1 librrd-dev \
                                                  libatk-bridge2.0-0 libgtk-3-0 libxrandr2 libasound2 libgbm1 \
                                                  libxdamage1 libxi6 libxtst6 libnss3 libcups2 libatk1.0-0 \
                                                  postgresql postgresql-contrib librrd-dev libldap2-dev libsasl2-dev \
                                                  xvfb x11-utils firefox-esr
RUN wget https://github.com/mozilla/geckodriver/releases/download/v0.31.0/geckodriver-v0.31.0-linux64.tar.gz
RUN tar xzf geckodriver-v0.31.0-linux64.tar.gz
RUN mv geckodriver /usr/local/bin/.
