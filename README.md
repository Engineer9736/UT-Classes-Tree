# UT-Classes-Tree

This is a listing of all classes in UT99, displayed in tree format, including the packagename in front of each class. That way you can easily spawn things ingame.

This is the grep command that produced the data array (Thanks to [@FTPlus](https://github.com/FTPlus)), i modified the grep command so it also added the package name to the output.

`
grep -Ero "^class [^ ]*( (extends|expands) [^ ]*)?" * | sed -E "s/([^ ]*)\/([^ ]*)class ([^ ]*)( (extends|expands) ([^ ;]*);?)?/[\"\1\",\"\3\",\"\6\"],/"
`

This grep command has to be ran in a download of this repository: https://github.com/Engineer9736/UT99-Classes
