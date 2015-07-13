testing-plugins
===============

Some plugins created with [xEdit](https://github.com/TES5Edit) that are used for testing [libloadorder](https://github.com/WrinklyNinja/libloadorder) and [LOOT](https://github.com/LOOT) with a wide variety of possible load order combinations.

The following plugin types are present:

1. Master with no dependencies.
2. Master with a master file dependency.
3. Master with a different master file dependency.
4. Plugin with no dependencies.
5. Plugin with a master file dependency.
6. Plugin with a different master file dependency.
7. Plugin with a plugin file dependency.
8. Plugin with a different plugin file dependency.

All the Oblivion plugins are header-only, with empty author and description fields.

The Skyrim plugins all have empty author fields, but otherwise contain description fields and records as follows:

* `Blank.esm`: Description field value is `v5.0`. Contains 10 records.
* `Blank - Different.esm`: Empty description field. Contains 9 records.
* `Blank - Master Dependent.esm`: Empty description field. Contains 8 records. 4 records are overridden from `Blank.esm`.
* `Blank - Different Master Dependent.esm`: Empty description field. Contains 7 records. 4 records are overridden from `Blank - Different.esm`.
* `Blank.esp`: Empty description field. Contains 6 records.
* `Blank - Different.esp`: Empty description field. Contains 5 records.
* `Blank - Master Dependent.esp`: Empty description field. Contains 4 records. 2 records are overridden from `Blank.esm`.
* `Blank - Different Master Dependent.esp`: Empty description field. Contains 3 records. 2 records are overridden from `Blank - Different.esm`.
* `Blank - Plugin Dependent.esp`: Empty description field. Contains 2 records. 1 record is overridden from `Blank.esp`.
* `Blank - Different Plugin Dependent.esp`: Empty description field. Contains 1 record, overridden from `Blank - Different.esp`.

All records are minimal BPTD (Body Part Data) records, so that the Skyrim plugins are also compatible with the Fallout 3 and Fallout: New Vegas record formats.
