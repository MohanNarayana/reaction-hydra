Mailchimp Open Commerce's Authentication uses the [ORY Hydra][hydra] OAuth 2.0 & OpenID Connect
server, for authentication.

This project provides a configured Authentication installation using Docker Compose.
Ready for Open Commerce development.

### Part of the Mailchimp Open Commerce Platform

This application is a part of the MOC Platform and is designed to work
with other services. You can launch MOC and its dependencies with a
single command by using the [MOC Platform][moc-platform] development
installation.

#### [See the MOC Platform README to get started quickly.][moc-platform]

## Project Status

This project is supported by Mailchimp Open Commerce for local MOC development.
It is not intended to serve as a template for running Authentication in production.

* :white_check_mark: Suitable for local development
* :warning: Contains specific configuration for the MOC Platform.
* :boom: Not safe for production.

## Services

These services will be available when the project is started:

| Service                                                           | Description                                                                                                         |
| ----------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **[Authentication Public API][authentication-public-api]**<br>http://localhost:4444 | Authentication's public API. It can be exposed to the public internet.                                                       |
| **[Authentication Admin API][authentication-admin-api]**<br>http://localhost:4445   | Authentication's administration API. This is unprotected and should not be exposed to the internet without a secure gateway. |
| **[Authentication Token API][authentication-public-api]**<br>http://localhost:5555  | Service for the Authentication token user.                                                                                   |

[authentication-public-api]: http://localhost:4444
[authentication-admin-api]: http://localhost:4445
[authentication-token-api]: http://localhost:5555

## License

Copyright © Mailchimp Open Commerce

[ory/hydra][hydra] is licensed under
[Apache License 2.0](https://github.com/ory/hydra/blob/master/LICENSE)

[hydra]: https://github.com/ory/hydra
