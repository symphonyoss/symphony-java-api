[![Dependencies](https://www.versioneye.com/user/projects/5770f47919424d000f2e0095/badge.svg?style=flat-square)](https://www.versioneye.com/user/projects/5770f47919424d000f2e0095)
[![Build Status](https://travis-ci.org/symphonyoss/symphony-java-api.svg)](https://travis-ci.org/symphonyoss/symphony-java-client)
[![Validation Status](https://scan.coverity.com/projects/9112/badge.svg?flat=1)](https://scan.coverity.com/projects/symphonyoss-symphony-java-api)
[![Symphony Software Foundation - Active](https://cdn.rawgit.com/symphonyoss/contrib-toolbox/master/images/ssf-badge-active.svg)](https://symphonyoss.atlassian.net/wiki/display/FM/Active)
<a href="https://sonarqube.com/overview?id=org.symphonyoss.symphony%3Asymphony-java-api"><img src="https://www.sonarqube.org/assets/logo-31ad3115b1b4b120f3d1efd63e6b13ac9f1f89437f0cf6881cc4d8b5603a52b4.svg" title="SonarQube" width="80"/></a>

Symphony Java API
====================

##Requirements

####POM:

        <dependency>
            <groupId>org.symphonyoss.symphony</groupId>
            <artifactId>symphony-java-api</artifactId>
            <version>(Version)</version>
        </dependency>

####Certificates:

        Please contact your Symphony local administrator to obtain the necessary certificates
        for the user/service account being used to access the POD.

        Server Truststore = Contains server certs
        User Keystore = Symphony user client certificate

        Note: The latest version of the SymphonyClient object supports the ability to create custom HTTP Clients, which
        means you can bind different .p12 certs representing different BOT users.


####Required System Properties:

        -Dkeystore.password=(Pass)
        -Dtruststore.password=(Pass)
        -Dsessionauth.url=https://(pod-host).symphony.com:8444/sessionauth
        //Note: you may have local HSM vs pod
        -Dkeyauth.url=https://(pod-host).symphony.com:8444/keyauth
        -Dsymphony.agent.pod.url=https://(symagent-host).mdevlab.com:8446/pod
        -Dsymphony.agent.agent.url=https://(symagent-host).mdevlab.com:8446/agent
        -Dcerts.dir=/dev/certs/
        -Dtruststore.file=/dev/certs/server.truststore
        -Dbot.user=(user name)

##Examples
[see Examples Project](https://github.com/symphonyoss/symphony-java-sample-bots)


##API Docs
[API Documentation](http://symphonyoss.github.io/symphony-java-api/index.html)

## Contribute
This project was initiated at [IHS Markit](https://www.ihsmarkit.com) and has been developed as open-source from the very beginning.

Contributions are accepted via GitHub pull requests. All contributors must be covered by contributor license agreements to comply with the [Code Contribution Process](https://symphonyoss.atlassian.net/wiki/display/FM/Code+Contribution+Process).
