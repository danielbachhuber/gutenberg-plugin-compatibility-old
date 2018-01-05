# gutenberg-plugin-compatibility

Database of plugins and their compatibility with Gutenberg. A no-software prototype of [wordpress/gutenberg#4072](https://github.com/WordPress/gutenberg/issues/4072#issuecomment-355422208).

Each [issue](https://github.com/danielbachhuber/gutenberg-plugin-compatibility/issues) correlates with a specific plugin (title is the plugin slug). The labels indicate state of compatibility:

* [state:untested](https://github.com/danielbachhuber/gutenberg-plugin-compatibility/issues?q=is%3Aissue+is%3Aopen+label%3Astate%3Auntested) - Haven't yet been tested for Gutenberg compatibility.
* [state:compatible](https://github.com/danielbachhuber/gutenberg-plugin-compatibility/issues?q=is%3Aissue+is%3Aopen+label%3Astate%3Acompatible) - Tested and confirmed to be compatible with Gutenberg.
    * [compatible:non-editor](https://github.com/danielbachhuber/gutenberg-plugin-compatibility/issues?q=is%3Aissue+is%3Aopen+label%3Acompatible%3Anon-editor) - Compatible because functionality doesn't touch the editor experience.
    * [compatible:works-with](https://github.com/danielbachhuber/gutenberg-plugin-compatibility/issues?q=is%3Aissue+is%3Aopen+label%3Acompatible%3Aworks-with) - Compatible because it's been updated to work with Gutenberg, or the existing functionality already works.
* [state:incompatble](https://github.com/danielbachhuber/gutenberg-plugin-compatibility/issues?q=is%3Aopen+is%3Aissue+label%3Astate%3Aincompatible) - Tested to be incompatible with Gutenberg.
    * [incompatible:broken-features](https://github.com/danielbachhuber/gutenberg-plugin-compatibility/issues?q=is%3Aopen+is%3Aissue+label%3Aincompatible%3Abroken-features) - Incompatible because features are present in Gutenberg but broken.
    * [incompatible:missing-features](https://github.com/danielbachhuber/gutenberg-plugin-compatibility/issues?q=is%3Aopen+is%3Aissue+label%3Aincompatible%3Amissing-features) - Incompatible because existing features are missing in Gutenberg.

The description is free-form documentation of the research.
