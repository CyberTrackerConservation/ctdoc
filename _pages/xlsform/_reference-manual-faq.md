## Frequently Asked Questions

### Which backends support XlsForm?
CyberTracker supports [ODK Central](https://getodk.org/), [KoBoToolbox](https://kobotoolbox.org) and [Survey123](https://survey123.arcgis.com).

### Are CyberTracker extensions visible to other tools?
XlsForm extensions support custom columns by using the `namespaces` value in the `settings` sheet. Columns prefixed with `bind::ct:` are only used by CyberTracker and are ignored (but preserved) by other tools.
