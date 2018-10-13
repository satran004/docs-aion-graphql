# Installation

[AION GraphQL](https://github.com/satran004/aion-graphql) library is using Spring Boot framework to expose the API endpoint.

**System Requirements:**

> Java 10.x and later
>
> Ubuntu 16.04 LTS or later, Mac OS
>
> Aion Kernel Installed on a server

**Setup from Binary**

Download the latest release binary from [GitHub](https://github.com/satran004/aion-graphql/releases) repo.

`$> unzip aion-graphql-dist-[version].zip`

or

`$> tar xvf aion-graphql-dist-[version].tar`

Go to extracted folder aion-graphql-dist-\[version\]

Start GraphQL server

`$> bin/aion-graphql`

_on Windows :_

`bin\aion-graphql.bat`

**Note:** Make sure you start the server inside _aion-graphql-dist-\[version\]_  folder only. Starting server inside bin folder will not work.

**Build from Source**

**`git clone https://github.com/satran004/aion-graphql.git`**

**`$> ./gradlew clean build`**

_**To run**_ 

`$> rpc_endpoint=tcp://[kernel-host]:8547 ./gradlew bootRun`

If you want to test GraphQL API on the browser, try the following url

`http://[host]:[port]/playground.html`

After running the above command, GraphQL endpoint can be accessed through the following url from your application :

`http://[host]:[port]/graphql`

