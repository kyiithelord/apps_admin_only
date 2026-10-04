Apps Menu for Administrators Only
=================================

Overview
--------

This module limits the built-in Apps menu to users in Odoo's Settings /
Administration group (``base.group_system``). It updates the menu's group
assignment during installation. Users outside that group do not see the menu.

Compatibility
-------------

* Odoo version: 19.0
* Dependency: ``base``
* License: LGPL-3

Installation
------------

1. Place the ``apps_admin_only`` directory in an Odoo addons path.
2. Update the Apps list in Odoo.
3. Search for **Apps Menu for Administrators Only** and install it.

Usage
-----

There are no settings to configure. A user with the Settings /
Administration group can see the Apps menu. A user without that group cannot
see it. To check the result, sign in with one user of each type.

Scope
-----

The module changes the visibility of ``base.menu_apps`` by assigning its
``group_ids`` to ``base.group_system``. It does not modify model access rights,
record rules, or other menus. Users may still have permissions to perform
other administrative operations through their existing groups or modules.
