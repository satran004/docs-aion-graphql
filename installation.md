# Installation

[AION GraphQL](https://github.com/satran004/aion-graphql) library is using Spring Boot framework to expose the API endpoint.

**System Requirements:**

> Java 10.x and later
>
> Ubuntu 16.04 LTS or later, Mac OS
>
> Aion Kernel Installed on a server

**Build from Source**

**`git clone https://github.com/satran004/aion-graphql.git`**

**`$> ./gradlew clean build`**

_**To run**_ 

`$> rpc_endpoint=tcp://[kernel-host]:8547 ./gradlew bootRun`

If you want to test GraphQL API on the browser, try the following url

`http://[host]:[port]/playground.html`

After running the above command, GraphQL endpoint can be accessed through the following url from your application :

`http://[host]:[port]/graphql`

