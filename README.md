# Keycloak OpenId Connect Spring Boot Example

This is a Spring Boot app to test the Keycloak OpenID Connect Authorization Code flow.

## Prerequisites

The application uses Spring, which includes Java SDK 1.8+ and Apache Maven 3.2+.

## Setup

You can pull the source of this application and start configuring the parameters of your keycloak in `app/src/main/resources/application.yml`.

    - Make sure you replace `keycloak-client-id` and `keycloak-client-secret` with your keycloak configuration.

    - Also provide appropriate `<TOKEN_URL>`, `<AUTHORIZATION_URL>` & `<USERINFO_URL>`.

## Run the sample

Run the package from your terminal with

```sh
    mvn spring-boot:run
```

Your app is available at http://localhost:8082 and you should see the Login button. To begin the login process, click on it.

## What can I use these for

OpenID Connect is a perfect way to incorporate user authentication to your application, where you are relying on another party to handle user identity.

In this situation, Keycloak handles the identity of the users, allowing it faster to get up and running

## Single Sign On (SSO)

By integrating OpenID Connect via Keycloak, you are building a session that can be used to single sign-on from your custom app to other applications that your users can access via the Keycloak portal.

If you have any queries/you find any problems, please don't hesitate to raise an issue.
