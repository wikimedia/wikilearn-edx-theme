# Wikilearn edx theme

This theme is used to provide Wikimedia colours, logos and other customizations for the Open edX server deployed on the [learn.wiki](https://learn.wiki/)instance.

This theme requires the use of [edx-platform](https://github.com/wikimedia/edx-platform/tree/develop) as it builds on top of that repository and cannot be used indepedently on its own.

## Development Branching Strategy

The branching model we follow for the theme to streamline development and deployment is as follows:

| Branch             | Description                                                      |
|--------------------|------------------------------------------------------------------|
| `develop`          | Primary development branch; deployed to development, staging and then production environments.    |
| `<feature-branch>` | Used for new features or bug fixes; merged into `develop`.       |

## Deployment Scheme

We follow a three phase deployment strategy.

First, we deploy the develop branch to the Development Environment for testing and verification. 

Once everything looks good, we make a new release/tag and then deploy that release/tag to the staging environment which is a mirror of the production environment

Once everything is verified, we finally deploy to the production environment.

The servers are available live on the following urls:

| Environment   | LMS URL             | Studio URL              |
|---------------|---------------------|--------------------------|
| Development   | https://dev.learn.wiki/    | https://studio.dev.learn.wiki/ |
| Staging       | https://stage.learn.wiki/   | https://studio.stage.learn.wiki/ |
| Production    | https://learn.wiki/    | https://studio.learn.wiki/ |

