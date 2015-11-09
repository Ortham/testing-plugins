testing-plugins
===============

Some plugins that are used for testing [libespm2](https://github.com/WrinklyNinja/libespm2), [libloadorder](https://github.com/WrinklyNinja/libloadorder) and [LOOT](https://github.com/LOOT) with a wide variety of possible load order combinations.

## Morrowind Plugins

The Morrowind plugins are hand-made in a hex editor using the available documentation, and only the following plugins are available:

* `Blank.esm`: Description field value is `v5.0`. Contains 10 records.
* `Blank - Master Dependent.esm`: Empty description field. Contains 8 records. 4 records are identical to records in `Blank.esm`.
* `Blank.esp`: Empty description field. Contains 6 records.

All records are GMST records.

## Oblivion Plugins

The Oblivion plugins were created with [xEdit](https://github.com/TES5Edit). They are header-only, with empty author and description fields, apart from the following:

* `Blank.esm`: Description field value is `v5.0`. Contains 10 records, with one being an interior CELL.
* `Blank - Master Dependent.esm`: Empty description field. Contains 8 records. 4 records are overridden from `Blank.esm`.

All records are minimal BOOK records unless otherwise noted above.

## Skyrim Plugins

The Skyrim plugins were created with [xEdit](https://github.com/TES5Edit). They all have empty author fields, but otherwise contain description fields and records as follows:

* `Blank.esm`: Description field value is `v5.0`. Contains 10 records, with one being an interior CELL.
* `Blank - Different.esm`: Empty description field. Contains 9 records.
* `Blank - Master Dependent.esm`: Empty description field. Contains 8 records. 4 records are overridden from `Blank.esm`.
* `Blank - Different Master Dependent.esm`: Empty description field. Contains 7 records. 4 records are overridden from `Blank - Different.esm`.
* `Blank.esp`: Empty description field. Contains 6 records.
* `Blank - Different.esp`: Empty description field. Contains 5 records.
* `Blank - Master Dependent.esp`: Empty description field. Contains 4 records. 2 records are overridden from `Blank.esm`.
* `Blank - Different Master Dependent.esp`: Empty description field. Contains 3 records. 2 records are overridden from `Blank - Different.esm`.
* `Blank - Plugin Dependent.esp`: Empty description field. Contains 2 records. 1 record is overridden from `Blank.esp`.
* `Blank - Different Plugin Dependent.esp`: Empty description field. Contains 1 record, overridden from `Blank - Different.esp`.

All records are minimal BPTD (Body Part Data) records unless otherwise noted above, so that the Skyrim plugins are also compatible with the Fallout 3 and Fallout: New Vegas record formats.

The `Skyrim/Data` folder also contains a `Blank.bsa` and its accompanying `Blank.bsl`. These were created by the `Archive.exe` that is supplied with Skyrim's Creation Kit. The BSA contains only one file, which is the LICENSE file in this repository.
