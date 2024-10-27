# Title

This is the 1st paragraph of my file.

This is the 2nd paragraph of my file.

This is the 3rd paragraph of my file.  
This is the 3rd paragraph of my file.This is the 3rd paragraph of my file.This is the 3rd paragraph of my file.This is the 3rd paragraph of my file.

## Visual elements

### Bold

This is **bold** text.

### Iitalic

This is *italic* text.

### Quote

This is a quote:
> This this is a quote.  
> This is another quote.

### Code and formulas

#### Code phrase

This is a text with `void` code phrase.

#### Code block

This is a code block:
```
<data name="ErrorHeader" xml:space="preserve">
<value>Error</value>
</data>
```
```
def parse_android(xml_path):
    """Parse Android XML."""
    tree = ET.parse(xml_path)
    root = tree.getroot()

    strings = {}

    for child in root:
        if child.tag == "string" and child.attrib.get("translatable", "true") != "false":
            strings[child.attrib["name"]] = child.text

    return strings
    ```