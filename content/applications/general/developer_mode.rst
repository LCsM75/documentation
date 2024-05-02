.. _developer-mode:

===========================
Developer mode (debug mode)
===========================

The developer mode, also known as debug mode, unlocks access to advanced :ref:`tools
<developer-mode/tools>` and options in Odoo.

.. note::
   The developer mode is also available with :ref:`assets <frontend/framework/assets_debug_mode>`,
   which are used to debug JavaScript code, and with :ref:`tests assets
   <frontend/framework/tests_debug_mode>`, which are used to run test tours.

Activation
==========

To activate it, open the :guilabel:`Settings` app, scroll down to the :guilabel:`Developer Tools`
section, and click :guilabel:`Activate the developer mode`.

Once activated, the :guilabel:`Deactivate the developer mode` option becomes available.

.. image:: developer_mode/settings.png
   :alt: Activating the developer mode in the Settings app

.. tip::
   Open the **command palette** by pressing `Ctrl + K` or `Cmd ⌘ + K`, then type `debug` to
   activate the developer mode with assets or deactivate it.

To activate the developer mode **from anywhere in the database**, add `?debug=1` to the URL after
`/web` (e.g., `https://example.odoo.com/web?debug=1#action=menu&cids=1`). To deactivate it, use
`?debug=0` instead.

Use `?debug=assets` to activate the developer mode with assets and `?debug=tests` to activate it
with tests assets.

.. admonition:: Browser extension

   The `Odoo Debug <https://github.com/Droggol/OdooDebug>`_ browser extension adds an icon to toggle
   developer mode on or off from the browser's toolbar. It is available on the `Chrome Web Store
   <https://chromewebstore.google.com/detail/odoo-debug/hmdmhilocobgohohpdpolmibjklfgkbi>`_ and
   `Firefox Add-ons <https://addons.mozilla.org/firefox/addon/odoo-debug/>`_.

.. _developer-mode/tools:

Developer tools
===============

Once the developer mode is activated, the developer tools can be accessed by clicking the
:icon:`fa-bug` :guilabel:`(bug)` icon. The menu contains tools useful for understanding or editing
technical data, such as the fields, filters, or actions of a view. The options available depend on
where it is accessed from.

.. image:: developer_mode/tools.png
   :alt: Accessing the developer tools
