# Exercise 1

1. Majority of the steps can be implemented in the CI via use of suitable github provided, or custom actions made and maintained by the users. For example, when it comes to building, linting and testing a react application, it is more than sufficient to use node action from github in order to run all the npm commands within the project. Some of the more complicated functionality might require to run either more complex cli commands within the pipeline config or use of the third party actions is needed (versioning of the project for example).

2. There is a sufficient amount of other alternatives to jenkins or github actions. Simple google search has shown quite an extensive list:
   Buddy.
   FinalBuilder.
   GoCD.
   IBM Urbancode.
   CircleCI.
   TeamCity.
   GitLab CI.
   Which includes both cloud and self-hosted solutions. Personally, I got to work with Gitlab CI and I was quite satisfied with its functionality and versatility as for the cloud solution.

3. Usually, self-hosted solutions are very versatile, but time-consuming when it comes to their setup. Cloud-based CI are simple and easy, but they can lack functionality. Majority of the web projects probably will be more than satisfied with the cloud based solution, however, if something more complicated is needed and there is a person within the team, who has experience with setting up a self-hosted pipeline -> it is worth setting it up. One case which comes to my mind is setting up a deployment job which requires vpn connection for instance (or 2FA). It is to my knowledge practically impossible to set it up via cloud based solution, though should be possible (but not easy), if self-hosted CI is implemented.
