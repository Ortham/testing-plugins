testing-plugins
===============

Some plugins that are to be used for testing libloadorder. They are all header-only, with empty author and description fields (excepting `Skyrim/Data/Blank.esm`, which has `v5.0` in its description field).

The following combinations are present:

1. Plugin with no dependencies.
2. Plugin with a master file dependency.
3. Plugin with a different master file dependency.
3. Plugin with a plugin file dependency.
3. Plugin with a different plugin file dependency.
4. Master with no dependencies.
5. Master with a master file dependency.
6. Master with a different master file dependency.

This should allow for a wide variety of possible load order combinations to be mocked, with missing masters, etc. implementable by renaming certain plugins.

Fallout 3, Fallout: New Vegas and Skyrim all use the same header format, so the plugins for Skyrim in this repository can also be used to test for other games too.
