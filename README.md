# Keycloak OpenId Connect Spring Boot Example

This is a Spring Boot app to test Keycloak OpenId Connect Authorization Code flow.

## Prerequisites

This application uses Spring which requires [Java SDK 1.8+](https://www.java.com/) and [Apache Maven 3.2+](https://maven.apache.org/).

## Setup

You can pull the source of this application and start configuring your keycloak parameters in `app/src/main/resources/application.yml`.

    - Make sure you replace `keycloak-client-id` and `keycloak-client-secret` with your keycloak configuration.

    - Also provide appropriate `<TOKEN_URL>`, `<AUTHORIZATION_URL>` & `<USERINFO_URL>`.

## Run the sample

Run the package from your terminal with

```sh
    mvn spring-boot:run
```

Your app will be available at http://localhost:8082 and you should see a Login Button. Click on that to start the login process.

## What can I use these for

OpenId Connect is a great way to add user authentication to your application where you are depending on another party to manage the user identities.

In this case Keycloak will manage the identity of your users making it faster to get up and running.

## Single Sign On (SSO)

By implementing OpenId Connect via Keycloak you are creating a session which can be used to single sign on from your custom app into other apps that your users may have access to via the Keycloak portal

If you have any queries / you notice any issues don't hesitate to raise issue.
