[![Dependencies](https://www.versioneye.com/user/projects/5770f47919424d000f2e0095/badge.svg?style=flat-square)](https://www.versioneye.com/user/projects/5770f47919424d000f2e0095)
[![Build Status](https://travis-ci.org/symphonyoss/symphony-java-api.svg)](https://travis-ci.org/symphonyoss/symphony-java-api)
[![Validation Status](https://scan.coverity.com/projects/9112/badge.svg?flat=1)](https://scan.coverity.com/projects/symphonyoss-symphony-java-api)
[![Symphony Software Foundation - Active](https://cdn.rawgit.com/symphonyoss/contrib-toolbox/master/images/ssf-badge-active.svg)](https://symphonyoss.atlassian.net/wiki/display/FM/Active)
<a href="https://sonarqube.com/overview?id=org.symphonyoss.symphony%3Asymphony-java-api"><img src="https://www.sonarqube.org/assets/logo-31ad3115b1b4b120f3d1efd63e6b13ac9f1f89437f0cf6881cc4d8b5603a52b4.svg" title="SonarQube" width="80"/></a>

Symphony Java API
====================

This project generates (swagger-gen) java client language binding(s) based on the Symphony LLC REST API specification.  Currently only the Jersey2 client implementation is generated, but this can be easily modified to support other variants. 

The generation will produce libraries for the three core REST API modules agent, authentication and pod.

Versioning of these bindings align with the Symphony LLC REST API versions.

Current releases include 1.45.0, 1.46.0 and 1.47.0-SNAPSHOT.  Javadoc is included in all maven distributions.






### POM for Jersey2 Bindings:

           <dependency>
                   <groupId>org.symphonyoss.symphony</groupId>
                   <artifactId>symphony-authenticator-java-jersey2-client</artifactId>
                   <version>${symphony-api-version}</version>
           </dependency>
           <dependency>
                   <groupId>org.symphonyoss.symphony</groupId>
                   <artifactId>symphony-agent-java-jersey2-client</artifactId>
                   <version>${symphony-api-version}</version>
           </dependency>
           <dependency>
                   <groupId>org.symphonyoss.symphony</groupId>
                   <artifactId>symphony-pod-java-jersey2-client</artifactId>
                   <version>${symphony-api-version}</version>
           </dependency>

### Branch Strategy:

Branch strategy aligns with spec versioning and merged into master for released version.  example branch format: 1_46, 1_47..etc


##API Docs
[API Documentation](http://symphonyoss.github.io/symphony-java-api/index.html)

## Contribute
This project was initiated at [IHS Markit](https://www.ihsmarkit.com) and has been developed as open-source from the very beginning.

Contributions are accepted via GitHub pull requests. All contributors must be covered by contributor license agreements to comply with the [Code Contribution Process](https://symphonyoss.atlassian.net/wiki/display/FM/Code+Contribution+Process).
