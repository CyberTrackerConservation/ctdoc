## Frequently Asked Questions

### Which backends support XmlForm?
CyberTracker can connect to ODK Central, KoBoToolbox and Survey123 (ArcGIS online).

### Are CyberTracker extensions visible to other tools?
The XlsForm extension system supports custom columns by using the `namespaces` value in the `settings` sheet. Unless these columns are specifically understood, they will be ignored. Columns prefixed with `bind::ct:` add behavior only in CyberTracker.