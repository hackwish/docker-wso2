FROM hackwish/ubuntu-java:oracle8

LABEL mantainer=hackwish

RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys '379CE192D401AB61'

RUN echo "deb https://dl.bintray.com/wso2/deb apim_260 release" | \
tee -a /etc/apt/sources.list

RUN apt-get update && \
apt-get install wso2am-2.6.0

EXPOSE 9443 9763 8243 8280 10397 7711
ENTRYPOINT ["wso2am-2.6.0"]
