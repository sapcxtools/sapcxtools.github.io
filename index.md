# SAP CX Tools

SAP CX tools is a set of tools and extensions that provide best-in-class enhancements of the standard CX products of SAP. These tools and extensions are not published nor maintained by SAP.

## SAP Commerce Extensions

All extensions available on [sapcx.tools][sapcxtools] are built with high test coverage and do not influence the behavior of your project without changes to your configuration. This is guaranteed and intended by design, because [sapcx.tools][sapcxtools] gives the full control of functionality into the hands of the project teams. Our coding conventions and code reviews follow high standards and decline features, that will change the standard behavior without activating them via a configuration parameter.

The following extensions are served and maintained by [sapcx.tools][sapcxtools].

### SAP Commerce Toolkit

The `sapcommercetoolkit` extension serves as the swiss army knife for SAP Commerce Cloud projects. Its core focusses on maintainability and controlling of ImpEx imports during system setup.

In addition, it provides enhancements for (local) development, such as a file or database storage for HTML emails sent by the platform, that lets you develop on email processes without ramping up an SMTP server. This is especially useful to avoid emails being sent out from (local) development environments. Also, the lightweight thymeleaf rendering engine for HTML emails replaces the rather heavy velocity rendering engine that requires the business process modeling for each and every email.

Still, the biggest benefit comes from its wide and continuously growing set of predefined test doubles (stubs, mocks, spies, and fakes) and builders for standard services and model classes. These help to write better and faster running unit tests without the need of heavy frameworks like Mockito.

More details on the `sapcommercetoolkit` can be found in its [README.md][sapcommercetoolkitreadme] file.

### SAP CX Backoffice

The `sapcxbackoffice` extension has three major features:

- A generic sync related items visitor, that lets you configure your relations for the actual sync status, instead of having to create and implement one item visitor per item type manually.
- Sort data locales by isocode to stop content editors from being embarrassed when maintaining content in multiple languages like `de` (master), `de_DE` (Germany), `de_CH` (Swiss), `de_AT` (Austria), etc.
- Limit available list of UI languages during login (and within the backoffice). The standard allows the login with every data locale available within the system, which does not make sense.

More details on the `sapcxbackoffice` can be found in its [README.md][sapcxbackofficereadme] file.

### SAP CX Environment Configuration

The `sapcxenvconfig` extension provides environment specific configuration to the Spartacus frontend, e.g. to configure single-sign-on scenarios based on OAuth2 etc. on an environment base.

More details on the `sapcxenvconfig` can be found in its [README.md][sapcxenvconfigreadme] file.

### SAP CX Reporting

The `sapcxreporting` extension provides reporting capabilities within the backoffice and for your business processes, e.g. letting your customers download a result list from the frontend as Excel file.

You can configure reports within the backoffice and run them periodically to send data reports to your business users, or use the SDK to create reports from your own project code.

More details on the `sapcxenvconfig` can be found in its [README.md][sapcxreportingreadme] file.

### SAP CX Single-Sign-On

The `sapcxsinglesignon` extension provides core implementations for SSO integration with external service and identity providers, such as [Auth0 by Okta][okta].

More details on the `sapcxsinglesignon` can be found in its [README.md][sapcxsinglesignonreadme] file.

## License

All SAP CX Tools extensions are licensed under the Apache 2.0 license.

A permissive license whose main conditions require preservation of copyright and license notices. Contributors provide an express grant of patent rights. Licensed works, modifications, and larger works may be distributed under different terms and without source code.

[View full Apache 2.0 License][license]

[sapcxtools]: https://www.sapcx.tools
[sapcommercetoolkitreadme]: https://github.com/sapcxtools/workspace/blob/main/hybris/bin/custom/sapcxtools/sapcommercetoolkit/README.md
[sapcxbackofficereadme]: https://github.com/sapcxtools/workspace/blob/main/hybris/bin/custom/sapcxtools/sapcxbackoffice/README.md
[sapcxenvconfigreadme]: https://github.com/sapcxtools/workspace/blob/main/hybris/bin/custom/sapcxtools/sapcxenvconfig/README.md
[sapcxreportingreadme]: https://github.com/sapcxtools/workspace/blob/main/hybris/bin/custom/sapcxtools/sapcxreporting/README.md
[sapcxsinglesignonreadme]: https://github.com/sapcxtools/workspace/blob/main/hybris/bin/custom/sapcxtools/sapcxsinglesignon/README.md
[okta]: https://www.okta.com/
[license]: https://choosealicense.com/licenses/apache-2.0/
