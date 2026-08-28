# STXT

**STXT** is a plain-text language for structured, semantic documents: no braces, no closing tags,
just indentation. It is designed to be equally readable by people and by machines, and it comes
with an optional schema layer so documents can be validated.

```stxt
# A comment
Document (com.example.docs): Title
	Metadata:
		Author: Joan
		Date: 2026-08-09
	Content >>
		Everything indented under a ">>" node is literal text:
		the #, : and >> inside are not interpreted.
```

Start at **<https://stxt.dev>** — the tutorial, the five specifications and the tools — or try it
directly in the browser at **<https://play.stxt.dev>**.

## The repositories

The specification is the first authority of the ecosystem: the implementations derive from it,
never the other way around.

```
specifications (stxt-lang)
  → stxt-impl  (neutral pseudocode)
      ├→ stxt-js      @stxt-lang/core on npm
      ├→ stxt-java    dev.stxt:stxt-core on Maven Central
      └→ stxt-python  stxt on PyPI
```

| Repository | Role |
|---|---|
| [stxt-lang](https://github.com/stxt-lang/stxt-lang) | The five normative specifications, the conformance kit and the source of the portal |
| [stxt-impl](https://github.com/stxt-lang/stxt-impl) | Neutral pseudocode of the implementation, second authority after the specifications |
| [stxt-js](https://github.com/stxt-lang/stxt-js) | TypeScript reference port, [`@stxt-lang/core`](https://www.npmjs.com/package/@stxt-lang/core) |
| [stxt-java](https://github.com/stxt-lang/stxt-java) | Java port, [`dev.stxt:stxt-core`](https://central.sonatype.com/artifact/dev.stxt/stxt-core) |
| [stxt-python](https://github.com/stxt-lang/stxt-python) | Python port, [`stxt`](https://pypi.org/project/stxt/) |
| [stxt-cli](https://github.com/stxt-lang/stxt-cli) | The `stxt` command, [`@stxt-lang/cli`](https://www.npmjs.com/package/@stxt-lang/cli) |
| [stxt-vscode](https://github.com/stxt-lang/stxt-vscode) | VS Code extension, [`stxt-lang.stxt`](https://marketplace.visualstudio.com/items?itemName=stxt-lang.stxt) |
| [stxt-play](https://github.com/stxt-lang/stxt-play) | The playground, <https://play.stxt.dev> |

## License

MIT © stxt-lang, across the whole organization.
