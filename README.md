# Spring Boot and React
This example app shows how to create a Spring Boot API and CRUD (create, read, update, and delete) its data with a React app.

Please read Use React and Spring Boot to Build a Simple CRUD App to see how this app was created.

Prerequisites: Java 11 and Node.js 16+

Okta has Authentication and User Management APIs that reduce development time with instant-on, scalable user infrastructure. Okta's intuitive API and expert support make it easy for developers to authenticate, manage, and secure users and roles in any application.

Getting Started
Links
Help
License
Getting Started
To install this example application, run the following commands:

git clone https://github.com/oktadev/okta-spring-boot-react-crud-example.git spring-react
cd spring-react
This will get a copy of the project installed locally. To install all of its dependencies and start each app, follow the instructions below.

To run the server, run:

./mvnw spring-boot:run
To run the client, cd into the app folder and run:

npm i && npm start
Create an Application in Okta
Before you begin, you'll need a free Okta developer account. Install the Okta CLI and run okta register to sign up for a new account. If you already have an account, run okta login.

Then, run okta apps create. Select the default app name, or change it as you see fit. Choose Web and press Enter.

Select Okta Spring Boot Starter. Accept the default Redirect URI of http://localhost:8080/login/oauth2/code/okta and use http://localhost:3000,http://localhost:8080 for the Logout Redirect URI.

The Okta CLI will create an OIDC Web App in your Okta Org. It will add the redirect URIs you specified and grant access to the Everyone group. You will see output like the following when it's finished:

Okta application configuration has been written to:
  /path/to/app/src/main/resources/application.properties
Open src/main/resources/application.properties to see the issuer and credentials for your app.

okta.oauth2.issuer=https://dev-133337.okta.com/oauth2/default
okta.oauth2.client-id=0oab8eb55Kb9jdMIr5d6
okta.oauth2.client-secret=NEVER-SHOW-SECRETS
NOTE: You can also use the Okta Admin Console to create your app. See Create a Spring Boot App for more information.

Run ./mvnw spring-boot:run -Pprod and log in to your app at http://localhost:8080.

Links
This example uses the following open source libraries:

React
Spring Boot
Spring Security
Help
Please post any questions as comments on the blog post, or visit our Okta Developer Forums.

License
Apache 2.0, see LICENSE.

About
Simple CRUD with React and Spring Boot 2.0

developer.okta.com/blog/2022/06/17/simple-crud-react-and-spring-boot
Topics
crud spring-boot authentication reactjs jpa csrf oidc csrf-protection
Resources
 Readme
License
 Apache-2.0 license
Code of conduct
 Code of conduct
Stars
 207 stars
Watchers
 12 watching
Forks
 139 forks
Releases 1
v1.0
Latest
on 6 Jun
Packages
No packages published
Contributors 6
@mraible
@dependabot[bot]
@rwinch
@cameronmoreau
@major1xu
@fatcatdog
Languages
Java
45.0%
 
JavaScript
44.1%
 
HTML
6.9%
 
CSS
4.0%
Footer
?? 2022 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
