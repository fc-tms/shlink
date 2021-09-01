FROM shlinkio/shlink

RUN apk update && apk add ca-certificates && rm -rf /var/cache/apk/*

ADD https://dl.cacerts.digicert.com/DigiCertGlobalRootCA.crt.pem /usr/local/share/ca-certificates/
ADD https://www.digicert.com/CACerts/BaltimoreCyberTrustRoot.crt.pem /usr/local/share/ca-certificates/
ADD https://www.d-trust.net/cgi-bin/D-TRUST_Root_Class_3_CA_2_2009.crt /usr/local/share/ca-certificates/

RUN update-ca-certificates
