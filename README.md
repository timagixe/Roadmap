# Metarhia subsystems

| Subsystem / Task                         | Priority | Maintainer                        | Comments                               |
| ---------------------------------------- | -------- | --------------------------------- | -------------------------------------- |
| Application server ([impress][impress])  | High     | [Timur Shemsedinov][tshemsedinov] | worker restart & stability             |
| Core modules                             | Medium   | [Timur Shemsedinov][tshemsedinov] | support                                |
| Ultra-thin isolation ([metavm][metavm])  | High     | [Timur Shemsedinov][tshemsedinov] | dependencies access control            |
| Lowcode runtime ([lowscript][lowscript]) | High     | [Timur Shemsedinov][tshemsedinov] | [md][md], [petri][petri]               |
| Scheduling                               | Medium   | [Timur Shemsedinov][tshemsedinov] | [cron][cron]: `0 5 * ? * * *`          |
| Schemas ([metaschema][metaschema])       | Critical | [Georg Oldenburger][georgolden]   | custom types, refactoring              |
| [OAuth 2.0][oauth2]                      | Critical |                                   | prerequisite for ESB                   |
| Enterprise bus ([openapi][openapi])      | Critical | [Timur Shemsedinov][tshemsedinov] | declarative service integration        |
| Storage multitenancy                     | Critical | [Georg Oldenburger][georgolden]   | sharding key, tenant id                |
| Application multitenancy                 | Critical | [Timur Shemsedinov][tshemsedinov] | impress as virtual hosting             |
| Deploy automation                        | Medium   |                                   | `git pull` and restart                 |
| Health monitoring                        | Medium   |                                   | Logs, profiling, metrics               |
| Payment integration                      | Medium   |                                   | [Paypal][paypal], [Stripe][stripe]     |
| Green threads                            | Medium   | [Timur Shemsedinov][tshemsedinov] | [noroutine][noroutine]                 |
| File storage                             | Medium   |                                   | [S3][s3], [MinIO][minio]               |
| Mail subsystem                           | Medium   |                                   | [metamail][metamail]                   |
| Report generator                         | Medium   |                                   | [LaTeX][latex], [pdfmake][pdfmake]     |
| Message queue                            | Medium   | [Timur Shemsedinov][tshemsedinov] | [Redis BULL][bull], [metacom][metacom] |
| Form generator                           | Medium   | [Leon Polak][leonpolak]           |                                        |
| Admin panel                              | Medium   | [Leon Polak][leonpolak]           |                                        |
| WEB IDE                                  | Medium   | [Leon Polak][leonpolak]           |                                        |
| Frontend framework                       | Medium   | [Roman Ohiievych][rohiievych]     | [swayer][swayer]                       |
| Metacom: send events to server           | Medium   | [Roman Ohiievych][rohiievych]     |                                        |
| Metacom: streams                         | Low      | [Roman Ohiievych][rohiievych]     |                                        |
| Metacom transport: ws, http2, tcp, tls   | Low      |                                   |                                        |
| Computation (Spreadsheet)                | Low      | [Timur Shemsedinov][tshemsedinov] | js reactive expressions                |
| Metarhia CLI                             | Low      |                                   | generate app, api etc.                 |
| Orchestration                            | Low      | [Timur Shemsedinov][tshemsedinov] | [metacom][metacom] between peers       |
| Double-entry accounting                  | Low      |                                   | reactive js expressions                |
| PG migrations                            | Paused   |                                   |                                        |
| Application firewall                     | Paused   |                                   |                                        |
| Load balancer                            | Paused   |                                   |                                        |
| Globalstorage                            | Paused   | [Timur Shemsedinov][tshemsedinov] | distributed storage                    |

## Timeline

| Critical | High   | Medium  | Low         | Paused |
| -------- | ------ | ------- | ----------- | ------ |
| 14 May   | 21 May | 11 June | End of 2022 |        |

[impress]: https://github.com/metarhia/impress
[metavm]: https://github.com/metarhia/metavm
[lowscript]: https://github.com/metarhia/lowscript
[metaschema]: https://github.com/metarhia/metaschema
[noroutine]: https://github.com/metarhia/noroutine
[metamail]: https://github.com/metarhia/metamail
[swayer]: https://github.com/metarhia/swayer
[metacom]: https://github.com/metarhia/metacom
[oauth2]: https://oauth.net/2/
[tshemsedinov]: https://github.com/tshemsedinov
[leonpolak]: https://github.com/leonpolak
[georgolden]: https://github.com/georgolden
[rohiievych]: https://github.com/rohiievych
[md]: https://daringfireball.net/projects/markdown/
[petri]: https://en.wikipedia.org/wiki/Petri_net
[cron]: https://en.wikipedia.org/wiki/Cron
[openapi]: https://github.com/metarhia/impress/issues/1733
[s3]: https://aws.amazon.com/s3/
[minio]: https://min.io/
[latex]: https://www.latex-project.org/
[pdfmake]: https://www.npmjs.com/package/pdfmake
[bull]: https://github.com/OptimalBits/bull
[paypal]: https://www.paypal.com/
[stripe]: https://stripe.com/
