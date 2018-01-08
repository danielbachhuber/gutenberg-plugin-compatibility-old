# gutenberg-plugin-compatibility

Database of plugins and their compatibility with Gutenberg. A no-software prototype of [wordpress/gutenberg#4072](https://github.com/WordPress/gutenberg/issues/4072#issuecomment-355422208).

_Compatible_ means a WordPress user can use the Gutenberg editor with the plugin. For instance, [Akismet is compatible](https://github.com/danielbachhuber/gutenberg-plugin-compatibility/issues/1) with Gutenberg because it doesn't expose any UI in the editor. However, [Shortcodes Ultimate is incompatible](https://github.com/danielbachhuber/gutenberg-plugin-compatibility/issues/40) because the media button it adds to the classic editor isn't present in Gutenberg.

Compatible really means that a WordPress user should not lose any functionality when they update to WordPress 5.0 on day one.

## Testing

All testing is performed on a stock WordPress install.

For each plugin:

1. Install and activate the plugin on the install.
2. Open a post in the classic editor in one tab, and the Gutenberg editor in another tab.
3. Compare the before (classic editor) to after (Gutenberg) to determine whether the plugin is compatible.

Once you've made your determination, record your results according to the data format below.

## Data Format

Each [issue](https://github.com/danielbachhuber/gutenberg-plugin-compatibility/issues) correlates with a specific plugin.

The **title is the plugin slug**. The **labels indicate state of compatibility**:

* [state:untested](https://github.com/danielbachhuber/gutenberg-plugin-compatibility/issues?q=is%3Aissue+is%3Aopen+label%3Astate%3Auntested) - Haven't yet been tested for Gutenberg compatibility.
* [state:compatible](https://github.com/danielbachhuber/gutenberg-plugin-compatibility/issues?q=is%3Aissue+is%3Aopen+label%3Astate%3Acompatible) - Tested and confirmed to be compatible with Gutenberg.
    * [compatible:non-editor](https://github.com/danielbachhuber/gutenberg-plugin-compatibility/issues?q=is%3Aissue+is%3Aopen+label%3Acompatible%3Anon-editor) - Compatible because functionality doesn't touch the editor experience.
    * [compatible:works-with](https://github.com/danielbachhuber/gutenberg-plugin-compatibility/issues?q=is%3Aissue+is%3Aopen+label%3Acompatible%3Aworks-with) - Compatible because it's been updated to work with Gutenberg, or the existing functionality already works.
* [state:incompatble](https://github.com/danielbachhuber/gutenberg-plugin-compatibility/issues?q=is%3Aopen+is%3Aissue+label%3Astate%3Aincompatible) - Tested to be incompatible with Gutenberg.
    * [incompatible:broken-features](https://github.com/danielbachhuber/gutenberg-plugin-compatibility/issues?q=is%3Aopen+is%3Aissue+label%3Aincompatible%3Abroken-features) - Incompatible because features are present in Gutenberg but broken.
    * [incompatible:missing-features](https://github.com/danielbachhuber/gutenberg-plugin-compatibility/issues?q=is%3Aopen+is%3Aissue+label%3Aincompatible%3Amissing-features) - Incompatible because existing features are missing in Gutenberg.

The **description logs any and all research performed**. Reproducibility is important, yo.
