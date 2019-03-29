FROM hackwish/ubuntu-java:oracle8

LABEL mantainer=hackwish

RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys '379CE192D401AB61'

RUN echo "deb https://dl.bintray.com/wso2/deb ei_640 release" | \
tee -a /etc/apt/sources.list

RUN apt-get update && \
apt-get install wso2ei-6.4.0

EXPOSE 9443 9445 9446 9643 9763 8243 8280 10397 7711
ENTRYPOINT ["wso2ei-6.4.0-integrator", "wso2ei-6.4.0-broker", "wso2ei-6.4.0-business-process", "wso2ei-6.4.0-analytics-dashboard", "wso2ei-6.4.0-msf4j", "wso2ei-6.4.0-analytics-worker"]
