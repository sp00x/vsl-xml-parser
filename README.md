# vsl-xml-parser

A XML DOM-like parser implemented in VSL (Viz3 scripting language)

Implemented by Rune Bjerke (rune ÄT never DÖT no, or: rune @ Vizrt forums)

Version 1.0 - 2015-09-25

Copyright © never.no - but you're free to reuse this as long as you leave this notice in, or say hi on the Vizrt forums :P

Provided as-is, with no warranties as to if it works properly or not. You're to blame if you use this.

## Usage

See example usage in (test.txt), but basically:

* use ParseXml(xml, ignoreWhitespace, ignoreAdvanced) to parse the XML
* use FindElement() or FindElements() to find stuff/navigate
* use FlattenElement() to get text values

Not tested on a very high number of XML file samples, but should deal with the basics.

## Limitations

Does not really support:

* <!DOCTYPE ..> parsing (but somewhat gracefully deals with it)
* Name spaces (.Name will be e.g. ns:foo)
