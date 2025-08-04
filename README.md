# Custom Items
Repository of Custom Items for the needs of StalcraftHQ website

Contributions to be made via a PR, for approval by a developer or maintainer.

## Structure
The `listing.json` folder is NOT the format used by the [Official Item API](https://github.com/EXBO-Studio/stalcraft-database). The format of ScHQ items listing is streamlined for the website's requirements, and currently:
- Name Translations are simplified - the additional information is not required as deserializer relies on the property name instead.
- There's no Data Path or Icon Path - instead the location will be automatically inferred from `id` to corresponding `data` and `img` folders respectively.
- There's additional `key` property - this is used to determine the item type in a way that is compatible with data contained in [Official Item API](https://github.com/EXBO-Studio/stalcraft-database).
- `_variants` path for items is supported - it has to be placed in root of `data` folder the path inside is inferred from `id` property like Data Path and Icon Path, but otherwise works exactly the same as in [Official Item API](https://github.com/EXBO-Studio/stalcraft-database).

Data of specific item has the same format as items on [Official Item API](https://github.com/EXBO-Studio/stalcraft-database) due to the complexity and compatibility reasons.

### Structure notes
The structure is prone to change at any point to accomodate requirements of StalcraftHQ website without prior warning (except for permanent maintainers).  
The GitHub repository-based approach is subject for change or removal at any time.

## License
Copyright (c) 2025 StalcraftHQ & TehGM

Licensed under [GNU Affero General Public License v3.0](LICENSE) (GNU AGPL-3.0).
