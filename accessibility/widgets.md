---
layout: reference
title: widgets
requireCss: /static/less/cnqr-view/docs.less
---


<p><b>All widgets keyboard usage is based on <a href="http://www.w3.org/WAI/PF/aria-practices/#aria_ex">W3C standards</a></b></p>
<h3>Menu</h3>
<p>The menubar takes up one stop in the tab order, can be navigated with the following keyboard shortcuts:</p>
<ul>
	<li>If a menu bar item has focus and the menu is not open, then:
		<ul>
			<li><b>DOWN</b> - opens the menu and places focus on the first menu item in the opened menu or child menu bar.</li>
			<li><b>RIGHT/LEFT</b> - move focus to the adjacent menu bar item.</li>
		</ul>
	</li>

	<li>When a menu is open and focus is on a menu item in that open menu, then
		<ul>
			<li><b>UP</b> - cycle focus through the items in that menu.</li>
			<li><b>ESCAPE</b> - open menu or submenu and returns focus to the parent menu item.</li>
			<li><b>DOWN</b> - opens the submenu and puts focus on the first submenu item, If the menu item with focus has a submenu</li>
	   </ul>
	<li>First item in menu bar should be in the tab order (tabindex=0).</li>
	<li>Tabbing out of the menu component closes any open menus.</li>
	<li>With focus on a submenu item, the user must use arrows or the Escape key to progressively close submenus and move up to the parent menu item(s).</li>
	<li>At the top level, Escape key closes any sub menus and keeps focus at the top level menu.</li>
</ul>

<h3>Tabs</h3>
<p>The tablist takes up one tab stop in the tab order. It can be navigated with the following shortcuts:</p>
<ul>
	<li><b>UP/LEFT</b> - Move focus to the previous tab. If on first tab, moves focus to last tab. Activate focused tab after a short delay.</li>
	<li><b>DOWN/RIGHT</b> - Move focus to the next tab. If on last tab, moves focus to first tab. Activate focused tab after a short delay.</li>
	<li><b>HOME</b> - Move focus to the first tab. Activate focused tab after a short delay.</li>
	<li><b>END</b> - Move focus to the last tab. Activate focused tab after a short delay.</li>
	<li><b>SPACE</b> - Activate panel associated with focused tab.</li>
	<li><b>ENTER</b> - Activate or toggle panel associated with focused tab.</li>
</ul>

<h3>Dialogs</h3>
<p>The demo dialog is activated by clicking on the "Trigger Dialog" button.</p>
<p>When a modal dialog opens focus goes to the first focusable item in the dialog. Determining the first focusable item must take into account elements which receive focus by default (form fields and links) as well as items which may have a tabindex attribute with a positive value. If there is no focusable item in the dialog, focus is placed on the dialog container element.</p>
<p>While the dialog contains focus, the tab order will wrap inside the dialog. If the dialog is modal, it is not possible to move focus to the main page until the dialog is closed.</p>
<ul><li><b>ESCAPE</b> - open menu or submenu and returns focus to the parent menu item.</li></ul>

<h3>Autocomplete</h3>
<p>Typing into the text field will generate a dropdown list with auto-complete suggestions. The suggestions can be navigated using the arrow keys and selected using the Enter key.</p>
<p>Autocomplete feedback is provided through an ARIA live region. To be announced properly, it must be used with an ARIA compliant browser and a screen reader that runs in (auto) forms mode or application mode.</p>
<ul>
	<li><b>UP</b> - Move focus to the previous item. If on first item, move focus to the input.</li>
	<li><b>DOWN</b> - Move focus to the next item. If on the input, move focus to the first item.</li>
	<li><b>ESCAPE</b> - Close the menu.</li>
	<li><b>ENTER</b> - Select the currently focused item and close the menu.</li>
	<li><b>TAB</b> - Select the currently focused item, close the menu, and move focus to the next focusable element.</li>
	<li><b>PAGE UP</b> - Move focus to the first item in the menu</li>
	<li>/<b>PAGE DOWN</b> - Move focus to the last item in the menu</li>
</ul>


<h3>DatePicker...Coming Soon</h3>