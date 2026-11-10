# handify-theme

## Install

Edit `config/_default/module.yaml` to install the `handify-theme` module:

### V2

```yml
imports:
  - path: github.com/uncinq/handify-theme/v2
  - path: github.com/uncinq/hugolify-theme/v2
```

### V1

```yml
imports:
  - path: github.com/uncinq/handify-theme
  - path: github.com/uncinq/hugolify-theme
```

## Structured data

The theme adds the schema.org types of the building trades to the generic ones of hugolify-theme, through `layouts/_partials/func/GetSchemaTypesTheme.html`: `HomeAndConstructionBusiness`, `GeneralContractor`, `Electrician`, `Plumber`, `HVACBusiness`, `RoofingContractor`, `HousePainter` and `Locksmith`.

All of them are local businesses, descending from `HomeAndConstructionBusiness`: a trade without a type of its own (mason, tiler, carpenter, landscaper…) takes that one. Hugolify admin offers them for the organization, under *Config › Structured data*, and for each place. A site that defines its own hook replaces this list, see [Structured data](https://www.hugolify.io/docs/customization/structured-data/#types).

## Documentation

https://www.hugolify.io/docs/

## Licensing

Hugolify is free for personal or commercial projects (MIT license)
