Informational Header
====================

This is a HABPanel widget. It displays customizable, interactive notification items after the dashboard name.

![Example of a dashboard with informational-header](https://github.com/gersilex/informational-header/raw/master/screenshot.png "Example of a dashboard with informational-header")

Installation
------------

- Use the [HABPanel Widget Gallery](https://community.openhab.org/t/habpanel-widget-gallery/34691) and search for `gersilex/informational-header`.
- Click the import button.

-or-

- Download `informational-header.widget.json`
- Import it from the HABPanel settings interface

Configuration & Usage
---------------------

- Notifications should be separate items and be member of a group you set in &lt;Notifications Group Name>.
- Style the notification with Bootstrap3 button classes by adding one of these classes to your item's tags: \"btn-default\", \"btn-primary\", \"btn-success\", \"btn-info\", \"btn-warning\", \"btn-danger\".
- Give the buttons an additional glowing animation by adding \"glow\" to the item's tags in addition to the btn-color-classes.

See `examples/notifications.items` for a working example.

- Choose the custom widget as header replacement for one or more of your dashboards. Find instructions [in the official post on the openHAB Community forums](https://community.openhab.org/t/new-display-options-incl-experimental-custom-widgets-everywhere/34140)

![HABPanel configuration example](https://github.com/gersilex/informational-header/raw/master/example/HABPanel-Dashboard-settings.png)

Interactivity & Rules
---------------------

In the settings of the widget, you can choose a command to be sent, when you click or tap the notification. This can be used to fire rules that listen to `received command OFF` commands.

For example, you could stop a flood alarm, turn off your whole-house-audio system, reset energy meters or anything else that may need context-sensitive interaction.

Contributing
------------

Feel encouraged to open up issues on GitHub, fork, improve the code and discuss in the [official openHAB Community forums thread]()
