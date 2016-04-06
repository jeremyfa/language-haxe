# Haxe language support in Atom

This is an alternative `language-haxe` atom package based on https://github.com/theRemix/language-haxe

Even though some (not all) changes might end up in pull requests to the original package, this alternative package may be used _as is_, if it fits better some developers workflow.

### Differences with the original package

* The haxe syntax file was completely rewritten to be based on official atom javascript syntax file as they share a lot of similarities. This adds richer grammar and gives more theming possibilities.

* The new syntax file supports formatting of dom/xml/jsx elements in strings to work with projects like [haxe-react](https://github.com/massiveinteractive/haxe-react/issues/23)

* Every _framework-specific_ matching has been removed from the syntax file (no more hardcoded highlighting of flash/openfl API etc...).

* Many snippets have been removed/edited to match a different coding style/workflow. Ideally, they should be completely removed and put in another package, allowing for more flexibility depending on each developer preferences.

* Every syntax, snippet and configuration file is now refering to `source.hx` instead of `source.haxe`, because that's how it should be (for instance, javascript in atom uses `source.js`, not `source.javascript`).

* Indentation was slightly improved.
