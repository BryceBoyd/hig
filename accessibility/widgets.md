---
layout: reference
title: widgets
---

<p><b>All widgets keyboard usage is based on <a href="http://www.w3.org/WAI/PF/aria-practices/#aria_ex">W3C standards</a></b></p>

### Menu ###
The menubar takes up one stop in the tab order, can be navigated with the following keyboard shortcuts

* If a menu bar item has focus and the menu is not open, then:
 * **DOWN** - opens the menu and places focus on the first menu item in the opened menu or child menu bar.
 * **RIGHT/LEFT** - move focus to the adjacent menu bar item.
* When a menu is open and focus is on a menu item in that open menu, then
 * **UP** - cycle focus through the items in that menu.
 * **ESCAPE** - open menu or submenu and returns focus to the parent menu item.
 * **DOWN** - opens the submenu and puts focus on the first submenu item, If the menu item with focus has a submenu
  * First item in menu bar should be in the tab order (tabindex=0).
  * Tabbing out of the menu component closes any open menus.
  * With focus on a submenu item, the user must use arrows or the Escape key to progressively close submenus and move up to the parent menu item(s).
  * At the top level, Escape key closes any sub menus and keeps focus at the top level menu.</li>

### Tabs ###
The tablist takes up one tab stop in the tab order. It can be navigated with the following shortcuts
* **UP/LEFT** - Move focus to the previous tab. If on first tab, moves focus to last tab. Activate focused tab after a short delay.
* **DOWN/RIGHT** - Move focus to the next tab. If on last tab, moves focus to first tab. Activate focused tab after a short delay.
* **HOME** - Move focus to the first tab. Activate focused tab after a short delay.
* **END** - Move focus to the last tab. Activate focused tab after a short delay.
* **SPACE** - Activate panel associated with focused tab.
* **ENTER** - Activate or toggle panel associated with focused tab.

### Dialogs ###
The demo dialog is activated by clicking on the "Trigger Dialog" button.

When a modal dialog opens focus goes to the first focusable item in the dialog. Determining the first focusable item must take into account elements which receive focus by default (form fields and links) as well as items which may have a tabindex attribute with a positive value. If there is no focusable item in the dialog, focus is placed on the dialog container element.

While the dialog contains focus, the tab order will wrap inside the dialog. If the dialog is modal, it is not possible to move focus to the main page until the dialog is closed.

* **ESCAPE** - open menu or submenu and returns focus to the parent menu item.

### Autocomplete ###
Typing into the text field will generate a dropdown list with auto-complete suggestions. The suggestions can be navigated using the arrow keys and selected using the Enter key.

Autocomplete feedback is provided through an ARIA live region. To be announced properly, it must be used with an ARIA compliant browser and a screen reader that runs in (auto) forms mode or application mode.

* **UP** - Move focus to the previous item. If on first item, move focus to the input.
* **DOWN** - Move focus to the next item. If on the input, move focus to the first item.
* **ESCAPE** - Close the menu.
* **ENTER** - Select the currently focused item and close the menu.
* **TAB** - Select the currently focused item, close the menu, and move focus to the next focusable element.
* **PAGE UP** - Move focus to the first item in the menu
* **PAGE DOWN** - Move focus to the last item in the menu

### DatePicker...Coming Soon ###
