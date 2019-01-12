<p align="center">
  <img src="https://raw.githubusercontent.com/max-itup/content/master/assets/readme_logo.svg?sanitize=true" title="MaxItUp!">
</p>

<p align="center">
  <a href="https://max-itup.github.io/mac/" target="_blank" rel="noopener noreferrer">MaxItUp</a> is a tool to create a setup script for newly formatted Mac devices.
</p>

## Adding new content

This repository serves as the data container for **MaxItUp!**

### data.json

The json file contains two arrays for categories and items, changing this file will change the content in [website](https://max-itup.github.io/mac/)
```json
{
  "categories": [],
  "items": []
}
```

### Categories

To Add/update or delete categories, please use the following format:

```json
{
    "id": "Category unique identifier (string)",
    "name": "Category name (string)",
    "order": "Category order (int)"
}
```

### Items

To Add/update or delete items, please use the following format:

```json
{
    "id": "Item unique identifier (string)",
    "type": "Item type (cask, brew, gem, os_settings, ...) (string)",
    "name": "Item name (string)",
    "description": "Item description (optional string)",
    "category": "Category unique identifier (should be in categories array, string)",
    "download_url": "URL to download item (optional string)",
    "code": "Item code"
}
```

### Assets

When adding categories/items, please consider adding icons/background images for them

#### Categories

1. Image name: `category.id`
2. Image format : `.svg`
3. Location `/assets/categories`

#### Items

1. Image name: `item.id`
2. Image format : `.png`
3. Location `/assets/items`

## Thanks

Special thanks to:
- [Bashar Ghadanfar](https://github.com/lionbytes) coming up with the name **MaxItUp!** and designing the project's visual identity.

## License

MaxItUp is released under the MIT license. See [LICENSE](https://github.com/max-itup/content/blob/master/LICENSE) for more information.
