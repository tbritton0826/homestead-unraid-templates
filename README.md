# Homestead Unraid Templates

Official Unraid Community Applications metadata for Homestead. This repository
contains only the Unraid template and listing assets; the application source is
maintained in the [Homestead repository](https://github.com/tbritton0826/homestead).

## Container image

```text
ghcr.io/tbritton0826/homestead:latest
```

The listing installs the Homestead Free preview for one owner and one active
stream. Keep `/mnt/user/appdata/homestead` backed up before updating.

## Persistent recipes

The template maps `/mnt/user/Recipes` to `/media/recipes` and sets
`HOMESTEAD_RECIPES_DIR=/media/recipes`. Homestead writes portable recipe metadata
and artwork there. Reuse this mapping after reconfiguring the server.

Existing containers need both settings added through **Edit**; pulling a new
image does not add volume mappings. Keep the old appdata mapping when first
opening Recipes so existing recipes and photos can be migrated. Back up the
Recipes share separately. See [recipe preservation and recovery](https://github.com/tbritton0826/homestead/blob/main/RECIPE-STORAGE.md).

## Community Applications submission

Submit this repository URL at <https://ca.unraid.net/submit>, then run Validate
and Scan:

```text
https://github.com/tbritton0826/homestead-unraid-templates
```

The MIT license in this repository applies only to its template metadata. It
does not grant rights to the Homestead application or container image.
