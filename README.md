# Custom Items
Repository of Custom Items for the needs of StalcraftHQ website

Contributions to be made via a PR, for approval by a developer or maintainer.

## Structure
Custom items are divided by folders according to which section of the website they're used on.

Inside of each folder, there's a `listing.json` file. It is NOT the format used by the [Official Item API](https://github.com/EXBO-Studio/stalcraft-database). The format of ScHQ items listing is streamlined for the website's requirements, and currently:
- Name Translations are simplified - the additional information is not required as deserializer relies on the property name instead.
- There's no Data Path or Icon Path - StalcraftHQ client code infers the locations based on item ID.
- There's additional `key` property - this is used to determine the item type in a way that is compatible with data contained in [Official Item API](https://github.com/EXBO-Studio/stalcraft-database)
- Currently there's no `_variants` path for items - all custom items are assumed to be level 0.

Data of specific item has the same format as items on [Official Item API](https://github.com/EXBO-Studio/stalcraft-database) due to the complexity and compatibility reasons.

### Structure notes
The structure is prone to change at any point to accomodate requirements of StalcraftHQ website without prior warning (except for permanent maintainers).  
The GitHub repository-based approach is subject for change or removal at any time.

## License
Copyright (c) 2025 TehGM

Licensed under [GNU Affero General Public License v3.0](LICENSE) (GNU AGPL-3.0).
