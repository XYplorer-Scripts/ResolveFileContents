# ResolveFileContents

**Script to resolve variables within the selected file in
[XYplorer](http://xyplorer.com/index.php).**

This script reads the selected items, interpolates variables within their
contents, and writes the resolved content to sibling files with a '_resolved'
suffix.

One useful scenario for this is to place templates containing variables within
the [New Items menu](http://www.xyplorer.com/highlights.php#newitems) and use
it as normal. Then after using *New Items* this script can be run on the
created files to create copies of those items with the variables resolved.

----------

#### Details

The interpolation of variables is done using XYplorer's *Set* command with the
*reprocess* flag to enable post-processing. This should resolve any environment
variables, native XYplorer variables, and permanent variable within the file
contents.

To ensure the maximum number of variables are available for use this script
manipulates the selection so that the common `<cur*>` as well as the
`<prop>` can return appropriate values for each individual file. By default an
instant color filter will be applied to highlight which file is currently being
transformed.

When all items have been processed the script will attempt to restore the
original selection (included focused item) and any existing color filters.


----------

#### Usage
1. [Download](https://github.com/XYplorer-Scripts/ResolveFileContents/releases/latest)
2. Select files containing variables.
3. Run *ResolveFileContents.xys*.

#### Requires
+ XYplorer with scripting enabled.

#### Tested On
+ Microsoft Windows 7 Professional SP1 x64
+ XYplorer v16.20.0300

#### Notes
+ Developed in response to this
[question](http://www.xyplorer.com/xyfc/viewtopic.php?f=3&t=15467).
+ Developed by [TheQwerty](https://github.com/TheQwerty) -
[contact](http://www.xyplorer.com/xyfc/memberlist.php?mode=viewprofile&u=438).

----------



_This is an unofficial script file for
[XYplorer](http://xyplorer.com/index.php) - a powerful file manager for
Windows.<br>
It has been released by a group of individuals under the collective
organization name [XYplorer-Scripts](https://github.com/XYplorer-Scripts)._
