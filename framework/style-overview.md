## Gateway Style Overview ##

The Gateway style uses a number of building blocks to generate the desired user experience. They are

* **Bootstrap** A User Experience frameworkoriginally developed by Twitter. It is composed of javascript, css, widgets, and a font that contains icon glyphs.
* **.LESS** LESS is composed of two parts:

* **A CSS extension syntax** providing dynamic behavior such as variables, mixins, operations and functions.
* **A CSS preprocessor** An engine that reads files with a .LESS extension and returns to the browser well-formed CSS. The LESS preprocessor was originally written in JavaScript, it can be run client side or server side.

Bootstrap's CSS is available in .LESS format and is fully parameterized, which makes it very easy to customize.

* **JQuery** A multi-browser JavaScript library designed to simplify the client-side scripting of HTML
* **JQueryUI** A collection of widgets built using JQuery

### CSS naming conventions ###

All class names should have semantic meaning, be lowercase, with a "-" dash character as word seperator (no CamelCase or _underscores). Because we are assimilating styles from three sources (Boostrap and JQeryUI plus our own styles), it is useful to understand the naming conventions used by each

* **Concur** - Classes are prefixed with "cnqr-"
* **JQueryUI** - Classes are prefixed with "ui-"
* **Boostrap** - Boostrap maintains that prefixing thier classes breaks the semantic organization of thier class structure, and refuse to provide a prefix.

### Default (third-party) vs. Override vs. Custom ###
<img src="/static/images/docs/less-dir-structure.png" class="pull-right" />

* **Default (third-party)** - this is the style unaltered provided directly from the third-party source. For Boostrap, these files live at \static\_third-party\bootstrap-3.3.1\less\
* **Override** - When we take an exising class, variable or mix-in from a third-party and redefine it. For Boostrap, these files live at \static\less\cnqr-bootstrap-3.3.1\override\
* **Custom**  - When we take a concept from a third-party class, variable or mixin, and make our own unique creation that does not have an analogous partner in the third-party library. For Boostrap, these files live at \static\less\cnqr-bootstrap-3.0.0\custom\