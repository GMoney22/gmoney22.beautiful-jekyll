{
    "title": "Server Profiles Roadmap",
    "description": "Server profiles optimize servers to perform specific tasks or functions.",
    "isversioned": false,
    "version": "",
    "islatestversion": false,
    "tags": ["whmadvanced", "webmail", "databases", "dns"],
    "layout": "article",
    "feature": "general-systems-administration",
    "weight": "",
    "id": "3af3a53ff05ede28acb5a8724d47f736"
}

## Overview

In cPanel & WHM version 76, we introduced WHM's [_Server Profile_](/whm/server-configuration/server-profile) interface (_WHM >> Home >> Server Configuration >> Server Profile_). Server profiles optimize servers to perform specific tasks or functions. These servers can host accounts that do not need certain applications. Each profile enables and disables a set of roles. Each role allows or disallows certain services related to the server's task. For example, a server that runs a *Mail Node* profile only enables services essential to mail. The profile disables all other services, such as Web Disk and FTP.

* For more information about server profiles, read our [How to Use Server Profiles](/knowledge-base/general-systems-administration/how-to-use-server-profiles) documentation.
* For information about linked server nodes, read our [cPanel Linked Nodes Guide](/knowledge-base/general-systems-administration/cpanel-linked-nodes-guide/) documentation.

<img src="/img/server-roadmap-arrow.png" alt="Roadmap">

*A visual representation of the phases.*

## Phases

This project has several phases. Each phase will deliver more server profile improvements, functions, and controls. You can read about each phase in the following section:

| Phase | Description | Notes | Status |
| ----- | ----------- | ----- | ------ |
| 1     | Introduce server profiles | <ul><li>We introduced the *Standard Node*, *Mail Node*, *Database Node*, and *DNS Node* server profiles. These profiles let you optimize a server for a specific task or function.</li><li>Each profile enables and disables a set of roles. Each role allows or disallows specific services that relate to the server's task.</li></ul>  | **Complete**     |
| 2     | Improve email deliverability | <ul><li>Improve how a server will deliver, receive, and process email.</li><li>We added WHM's [_Email Deliverability_](/cpanel/email/email-deliverability-in-cpanel) interface (_WHM >> Home >> Email >> Email Deliverability_). This interface helps you identify and fix any problems with your server’s DKIM, SPF, and PTR records.</li></ul> | **Complete**     |
| 3     | Manage API Tokens in cPanel | <ul><li>We introduced cPanel API tokens.</li><li>Users can issue these API tokens in cPanel's [_Manage API Tokens_](/cpanel/security/manage-api-tokens-in-cpanel) interface (_cPanel >> Home >> Security >> Manage API Token_). This feature lets users create, list, update, and revoke API tokens.</li></ul>  | **Complete** |
| 4     | Standalone *DNS Node* licensing | Support of *DNS Node* licenses. | **Complete**  |
| 5     | Link a new *Standard Node* to a new *Mail Node* server | <ul><li>Allow new cPanel accounts on a *Standard Node* server to connect to a *Mail Node* server.</li><li>Assign the mail tasks for new cPanel accounts to a different server.</li><ul> | **Complete**  |
| 6     | Transfer existing linked cPanel accounts between nodes | <ul><li>Support for transfers to and from a server with attached nodes.</li><li>Provide the ability to back up accounts with data from all of your server nodes.</li><li>Preserve a node setting when you transfer an account from one server to another.</li><ul> | **Complete** |
| 7     | Modify a cPanel account to offload mail | Offload a cPanel account's mail storage to a [linked node](/knowledge-base/cpanel-product/cpanel-glossary/#linked-node) in WHM's [*Modify an Account*](/whm/account-functions/modify-an-account) interface (*WHM >> Home >> Account Functions >> Modify an Account*). | **Complete** |
| 8     | Modify a cPanel account to host mail locally | Modify a [distributed cPanel account](/knowledge-base/cpanel-product/cpanel-glossary/#distributed-cpanel-account) to use only the local server in WHM's [*Modify an Account*](/whm/account-functions/modify-an-account) interface (*WHM >> Home >> Account Functions >> Modify an Account*). | **Complete** |
| 9      | Production Ready | Support a linked [child node](/knowledge-base/cpanel-product/cpanel-glossary#child-node) server with a [*Standard Node*](/knowledge-base/general-systems-administration/how-to-use-server-profiles#standard-node) or [*Mail Node*](/knowledge-base/general-systems-administration/how-to-use-server-profiles#mail-node) server profile in a production environment. | **Complete** |
| 10     | Future plans | Performance and optimizations. | **In progress** |
