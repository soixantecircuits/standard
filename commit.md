# Commiting is caring

A well written commit helps you to think about what you have done and how you want other to read it.
It is like a journal, a hourly log. It needs to be clear, readable and made for other.
If you care about your team members, you should write clear commit.

## Do

- Start with an emoji 
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