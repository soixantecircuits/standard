# Commit style

_Committing is caring_

A well written commit helps you to think about what you have done and how you want other to read it.
It is like a journal, a hourly log. It needs to be clear, readable and made for other.
If you care about your team members, you should write clear commit. Please use english.

## Do

- Start with an emoji
- Use English in your sentence
- Start with a lowercase
- Continue with an action verb
- Use the Present form
- Imply an issue, or ticket number, if one exist (it should)
- Specify the details : what did you fix, how did you fix it


```
git commit -am "📚 write documentation about app initialization"
git commit -am "🔥 clear memory after reload videos, fixes #32"
git commit -am "🎨 make a bigger typo and rounded button blue buttons, fixes #212"
git commit -am "💎 add rescale feature for picture canvas. Save it as dataToUrl, fixes #452"
git commit -am "🔥🐛 avoid jittering and remove flick effect, fixes #55"
git commit -am "➕📦 add three package"
git commit -am "👻 add .vscode to gitignore"
git commit -am "⚙ update port settings, fixed #342"
```

## Don't

```
git commit -am "writing documentation about something"
git commit -am "cleared memory"
git commit -am "🎨 fix bug 24"
git commit -am "💎 some changes"
git commit -am "avoiding effect, fixes #55"
git commit -am "added a package"
git commit -am "update gitignore"
git commit -am "change setting"
```

## Emoji references

### Priority emoji

* 📚 `:books:` when adding docs
* ✍️ `:writing_hand:` when updating a doc
* 💎 `:gem:` when adding a feature
* 🎨 `:art:` when styling the application, colors, shape, position
* 🖼 `:framed_picture:` when adding assets, like icons, images, etc.
* 📦 `:package:` when adding a dependency
* 🚀 `:rocket:` when improving performance
* 🐛 `:bug:` when fixing a bug
* 🔥 `:fire:` when removing code or files
* 🚧️️ `:construction:` when commiting a WIP
* 🚱 `:non-potable_water:` when plugging memory leaks
* 🔈 `:speaker:` when adding logging
* 🔇 `:mute:` when reducing logging

### Secondary emoji

* ✅ `:white_check_mark:` when adding a test
* 🔒 `:lock:` when dealing with security
* ⬆️ `:arrow_up:` when upgrading dependencies
* ⬇️ `:arrow_down:` when downgrading dependencies
* 👕 `:shirt:` when removing linter warnings

### Least emoji

* 🐧 `:penguin:` when fixing something on Linux
* 🍎 `:apple:` when fixing something on macOS
* 🏁 `:checkered_flag:` when fixing something on windows
