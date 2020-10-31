# Getting Started

Welcome to Notes, a demonstration project created by Warren Anderson to 
implement Docsify and using the docs-as-code philosophy, sometimes referred to as docs-like-code.
Other products like GitBook and MkDocs are also a great choices.

## Releases

A new release of the documentation is produced with every change of the major or minor number <span style="text-decoration: underline;">1<span>.<span style="text-decoration: underline;">0</span>.x in a release of the Notes backend server.
  
## AAAEmail-Code-Token

The dude  APIs implement an **Email-Code-Token** mechanism for authentication using **[jsonwebtoken](https://www.npmjs.com/package/jsonwebtoken)**.

1. Prompt the user for their **Email Address** and call POST /user/code. The endpoint will send a **Code** to the email address and respond with status=201.

1. Prompt the user for their **Code** and send it to GET /user/token. The endpoint will respond with a **Token** and status=200.

The **Token** must be used to authenticate all other endpoints.

Try the **Email-Code-Token** mechanism using Insomnia. See the **[Insomnia](/#Insomnia)** section of this guide for more information.
