# SAP CX Tools

SAP CX tools is a set of tools and extensions that provide best-in-class enhancements of the standard CX products of SAP. These tools and extensions are not published nor maintained by SAP.

## SAP Commerce Extensions

All extensions available on [sapcx.tools][sapcxtools] are built with high test coverage and do not influence the behavior of your project without changes to your configuration. This is guaranteed and intended by design, because [sapcx.tools][sapcxtools] gives the full control of functionality into the hands of the project teams. Our coding conventions and code reviews follow high standards and decline features, that will change the standard behavior without activating them via a configuration parameter.

The following extensions are served and maintained by [sapcx.tools][sapcxtools].

### SAP Commerce Toolkit

The `sapcommercetoolkit` extension serves as the swiss army knife for CCv2 projects. Its core focusses on maintainability and controlling of ImpEx imports during system setup.

In addition, it provides some enhancements for local development, such as a local-storage HTML email service, that lets you develop on mailing processes without ramping up a SMTP server.

The biggest benefit comes from its wide and continuously growing set of predefined test doubles (stubs, mocks, spies, and fakes) and builders for standard services and model classes. These help to write better and faster running unit tests without the need of heavy frameworks like Mockito.

More details on the `sapcommercetoolkit` can be found in its [README.md][readme] file.

## License

All SAP CX tools extensions are licensed under the GNU General Public License v3.0.

Permissions of this strong copyleft license are conditioned on making available complete source code of licensed works and modifications, which include larger works using a licensed work, under the same license. Copyright and license notices must be preserved. Contributors provide an express grant of patent rights.

![License overview](/assets/images/license_overview.png)

[View full GNU General Public License v3.0][license]

[sapcxtools]: https://www.sapcx.tools
[readme]: https://github.com/sapcxtools/extensions/blob/main/hybris/bin/custom/sapcxtools/sapcommercetoolkit/README.md
[license]: https://choosealicense.com/licenses/gpl-3.0/