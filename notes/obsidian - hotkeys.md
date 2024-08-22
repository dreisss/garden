---
created_at: 2024-08-22
tags: []
categories:
  - obsidian
  - hotkeys
aliases:
---
My custom hotkeys/shortcuts to [[obsidian]]:

[download!](https://raw.githubusercontent.com/dreisss/garden/main/.obsidian/hotkeys.json)

```dataviewjs
const hotkeysFile = await app.vault.readRaw(".obsidian/hotkeys.json");
const hotkeysJson = JSON.parse(hotkeysFile)

let hotkeysFormatted = []

for (let command in hotkeysJson) {
	let hotkey

	switch (typeof hotkeysJson[command][0]) {
		case "undefined":
			hotkey = ""
			break
		case "object":
			let modifiers = hotkeysJson[command][0]["modifiers"].join(" + ")
			let key = hotkeysJson[command][0]["key"]
			hotkey = `- [6] ${modifiers} + ${key}`
			break
	}

	hotkeysFormatted.push([command, hotkey])
}

dv.table(["Command", "Hotkey"], hotkeysFormatted.sort())
```

