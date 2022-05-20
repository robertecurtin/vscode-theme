# vscode-theme
thoughts and themes

Color Theme
===========

- What should stand out?
	- Variable names
	- Function names
	- Constants
	
- What should be less visible?
	- Certain keywords (if, else)
	- Types
	- *, ==, &, ->, .

- What should hide?
	- Boring keywords (static)

- Bright #F6019D #2DE2E6 #FF6C11 #FF3864

- Light #791E94 #920075

- Dark #261447 #023788 #650D89 #540D6E 

- "comments" light / 791E94
- "functions" light / 920075
- "keywords" dark / 261447
- "numbers" bright F6019D
- "strings" bright 2DE2E6
- "types" bright FF6C11
- "variables" bright FF3864

based off of Beeler's lua config, darkened:

```
	"editor.tokenColorCustomizations": {
		// "comments": "#00FF00",
		// "functions": "#00FF00",
		// "keywords": "#00FF00",
		// "numbers": "#00FF00",
		// "strings": "#00FF00",
		// "types": "#00FF00",
		// "variables": "#00FF00",
		"textMateRules": [
			// Order here matters
			// Variables, grey to avoid attention but clearly visible
			{ "scope":"variable", "settings": { "foreground": "#d0d0d0" } },
			{ "scope":"variable.language", "settings": { "foreground": "#d0d0d0" } },
			{ "scope":"variable.parameter", "settings": { "foreground": "#d0d0d0" } },
			{ "scope":"variable.other.member", "settings": { "foreground": "#d0d0d0" } },
			{ "scope":"variable.other.object", "settings": { "foreground": "#d0d0d0" } },
			{ "scope":"punctuation.definition.variable", "settings": { "foreground": "#d0d0d0" } },
			{ "scope":"entity.name.class", "settings": { "foreground": "#d0d0d0" } },
			// Comments, less visible than variables because they aren't usually useful
			{ "scope":"comment", "settings": { "foreground": "#7a7a7a" } },
			// Constants, eye-catching orange to draw attention to magic numbers
			{ "scope":"constant", "settings": { "foreground": "#bd764a" } },
			{ "scope":"constant.numeric", "settings": { "foreground": "#bd764a" } },
			{ "scope":"constant.language", "settings": { "foreground": "#bd764a" } },
			{ "scope":"constant.character.escape", "settings": { "foreground": "#bd764a" } },
			{ "scope":"constant.other", "settings": { "foreground": "#bd764a" } },
			{ "scope":"support.constant", "settings": { "foreground": "#bd764a" } },
			// String, soft green to stand out slightly without distracting
			{ "scope":"string", "settings": { "foreground": "#5bca61" } },
			// Character escapes in strings, slightly different to stand out from the rest of the string
			{ "scope":"constant.character.escape", "settings": { "foreground": "#42ffa7" } },
			// Functions, cyan to make it clearly different, but matches the "neutral" brightness
			{ "scope":"entity.name", "settings": { "foreground": "#47b4b6" } },
			{ "scope":"entity.name.function", "settings": { "foreground": "#47b4b6" } },
			{ "scope":"support.function", "settings": { "foreground": "#47b4b6" } },
			{ "scope":"support.module", "settings": { "foreground": "#47b4b6" } },
			{ "scope":"variable.function", "settings": { "foreground": "#47b4b6" } },
			// Invalid, bright orange to draw attention without being bright red
			{ "scope":"invalid.illegal", "settings": { "foreground": "#f69801" } },
			// Keyword, orange at "neutral" brightness so that it's clearly different but doesn't draw the eye
			{ "scope":"keyword", "settings": { "foreground": "#c27777" } },
			{ "scope":"keyword.control", "settings": { "foreground": "#c27777" } },
			{ "scope":"keyword.declaration", "settings": { "foreground": "#c27777" } },
			{ "scope":"storage.modifier", "settings": { "foreground": "#c27777" } },
			// Background information, less visible than variables because they don't matter, but not as hidden as comments
			{ "scope":"keyword.operator", "settings": { "foreground": "#bbbbbb" } },
			{ "scope":"punctuation.section", "settings": { "foreground": "#bbbbbb" } },
			{ "scope":"punctuation.terminator", "settings": { "foreground": "#bbbbbb" } },
			{ "scope":"punctuation.seperator.delimiter", "settings": { "foreground": "#ff0000" } },
			// Type, Pink to add color, mostly shows up in built-in types such as void
			{ "scope":"storage.type", "settings": { "foreground": "#ad4098" } },
			{ "scope":"storage.type.built-in", "settings": { "foreground": "#ad4098" } },
			{ "scope":"support.type", "settings": { "foreground": "#ad4098" } },
			{ "scope":"support.type.posix-reserved", "settings": { "foreground": "#ad4098" } },
			{ "scope":"support.class", "settings": { "foreground": "#ad4098" } },
			{ "scope":"entity.other.inherited-class", "settings": { "foreground": "#ad4098" } },
		],
	},

Light mode
Note that this has issues with some macros / functions being displayed as blue even though the scope inspector says they shouldn't be
				[
							// Order here matters
							// Variables, grey to avoid attention but clearly visible
							{ "scope":"variable", "settings": { "foreground": "#454545" } },
							{ "scope":"variable.language", "settings": { "foreground": "#454545" } },
							{ "scope":"variable.parameter", "settings": { "foreground": "#454545" } },
							{ "scope":"variable.other.member", "settings": { "foreground": "#454545" } },
							{ "scope":"variable.other.object", "settings": { "foreground": "#454545" } },
							{ "scope":"punctuation.definition.variable", "settings": { "foreground": "#454545" } },
							{ "scope":"entity.name.class", "settings": { "foreground": "#454545" } },
							// Comments, less visible than variables because they aren't usually useful
							{ "scope":"comment", "settings": { "foreground": "#909090" } },
							// Constants, eye-catching orange to draw attention to magic numbers
							{ "scope":"constant", "settings": { "foreground": "#cf611c" } },
							{ "scope":"constant.numeric", "settings": { "foreground": "#cf611c" } },
							{ "scope":"constant.language", "settings": { "foreground": "#cf611c" } },
							{ "scope":"constant.character.escape", "settings": { "foreground": "#cf611c" } },
							{ "scope":"constant.other", "settings": { "foreground": "#cf611c" } },
							{ "scope":"support.constant", "settings": { "foreground": "#cf611c" } },
							// String, soft green to stand out slightly without distracting
							{ "scope":"string", "settings": { "foreground": "#5bca61" } },
							// Character escapes in strings, slightly different to stand out from the rest of the string
							{ "scope":"constant.character.escape", "settings": { "foreground": "#42ffa7" } },
							// Functions, cyan to make it clearly different, but matches the "neutral" brightness
							{ "scope":"entity.name", "settings": { "foreground": "#47b4b6" } },
							{ "scope":"entity.name.function", "settings": { "foreground": "#47b4b6" } },
							{ "scope":"support.function", "settings": { "foreground": "#47b4b6" } },
							{ "scope":"support.module", "settings": { "foreground": "#47b4b6" } },
							{ "scope":"variable.function", "settings": { "foreground": "#47b4b6" } },
							// Invalid, bright orange to draw attention without being bright red
							{ "scope":"invalid.illegal", "settings": { "foreground": "#f69801" } },
							// Keyword, orange at "neutral" brightness so that it's clearly different but doesn't draw the eye
							{ "scope":"keyword", "settings": { "foreground": "#c27777" } },
							{ "scope":"keyword.control", "settings": { "foreground": "#c27777" } },
							{ "scope":"keyword.declaration", "settings": { "foreground": "#c27777" } },
							{ "scope":"storage.modifier", "settings": { "foreground": "#c27777" } },
							// Background information, less visible than variables because they don't matter, but not as hidden as comments
							{ "scope":"keyword.operator", "settings": { "foreground": "#808080" } },
							{ "scope":"punctuation.section", "settings": { "foreground": "#808080" } },
							{ "scope":"punctuation.terminator", "settings": { "foreground": "#808080" } },
							{ "scope":"punctuation.seperator.delimiter", "settings": { "foreground": "#ff0000" } },
							// Type, Pink to add color, mostly shows up in built-in types such as void
							{ "scope":"storage.type", "settings": { "foreground": "#ec4ccc" } },
							{ "scope":"storage.type.built-in", "settings": { "foreground": "#ec4ccc" } },
							{ "scope":"support.type", "settings": { "foreground": "#ec4ccc" } },
							{ "scope":"support.type.posix-reserved", "settings": { "foreground": "#ec4ccc" } },
							{ "scope":"support.class", "settings": { "foreground": "#ec4ccc" } },
							{ "scope":"entity.other.inherited-class", "settings": { "foreground": "#ec4ccc" } },
						]
```
