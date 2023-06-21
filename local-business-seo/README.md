
## Installation

1. Add the following to your site's `config.toml` to enable the `seo` module:

```toml
[module]
    [[module.imports]]
    path = "github.com/adammartelletti/hugo-modules/local-business-seo"
```

2. Add the following
   
```toml
[params.local]
  localBusinessName = "Re-Colour Windows"
  localBusinessImage = "/images/re-colour-logo.jpg"
  localBusinessTelephone = "+61 0438 563 143"
  localBusinessStreetAddress = "66 Le Grand Gardens, Marangaroo"
  localBusinessAddressLocality = "Perth"
  localBusinessAddressRegion = "WA"
  localBusinessPostalCode = "6064"
  localBusinessAddressCountry = "Australia"
  localBusinessLatitude = "-31.824229122889086"
  localBusinessLongitude = "115.83905325626318"
  localBusinessOpeningHours = "Mo,Tu,We,Th,Fr 07:00-17:00"
  ```

## Using Partial

Add the following to your site's `header.html`:

```
{{ partial "local-business-seo.html" . }}
```