cloudfoundry-sticky-session
===========================

Simple Java web app that prints Cloud Foundry environment variables and cookies and is useful to showcase sticky sessions.

It also lets you test the HealthManager by sending a "http://host/?shutdown=true" request.

To build, please use Maven from the root directory with the pom.xml file

    mvn package

which should generate a WAR file in the "target" directory.

If the app builds successfully, you should be able to push it to a Cloud Foundry environment by using `cf push` from the root directory that has the `manifest.yml` file.