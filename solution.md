# Web Engineering 2021-2022 / Lab2 RPC over HTTP

## Primary goal

Obviously, the first step is to deploy the server to wait for a client to connect.
I have used `./gradlew :server:build` and `./gradlew :server:bootRun` to build and run it respectively.

Then, while the server was running, I have executed the client using `./gradlew :client:build` and `./gradlew :client:bootRun` to build and run it respectively.

Apparently everything was working correctly, but the client showed an error explaining that something was wrong with the server.

So, I just needed to complete the code of the `Server.kt` that is responsible for returning the response to the client.
Also, I have modified the message that the `Client.kt` sends to finally get the expected result for the Primary goal.

## Github actions configuration

I have added the `work` branch in the `cy.yml` file to build the branch automatically using Github actions.