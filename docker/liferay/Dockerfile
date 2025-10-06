FROM liferay/dxp:latest

USER root

COPY fragments/frag-set fragments/liferay-deploy-fragments.json /tmp/fragments/

RUN apt-get update && \
apt-get install -y zip && \
zip -r /opt/liferay/deploy/frag-set.zip /tmp/fragments/*

USER liferay:liferay