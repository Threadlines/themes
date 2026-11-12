# Threadlines themes

These are themes people made for [Threadlines](https://www.threadlines.dev/?ref=themes-repo) and chose to share. Each one is a single `.threadlines-theme` file. It sets the app's colors, and it can carry its own fonts and a bit of slow live art that sits behind your threads.

## Browse

In Threadlines, open **Settings › Appearance › Showcase**. Try any theme on your own screen first. It only stays if you keep it.

## Share yours

From the app, open your theme's menu and pick **Share to Showcase…**. Threadlines forks this repo to your GitHub account and opens a pull request from it.

You can also do it by hand. Export your theme with **Export file…** in Threadlines, which leaves out private details and asks for your credit and license. Then fork this repo and add a folder under `themes/`. Name the folder with lowercase letters, digits and hyphens, 40 characters at most. Put three files in it:

```
themes/your-theme/theme.threadlines-theme   the file you exported
themes/your-theme/thumbnail.png             a 320×200 PNG picture of the theme
themes/your-theme/meta.json                 see below
```

```json
{ "sharedBy": "your-github-login" }
```

`sharedBy` must be the account that opens the pull request, or `null` if you'd rather not be named. Don't add `featured` (we set it), and don't write `NOTICE.md` or edit `index.json`: a workflow rebuilds both after each merge, and takes the date a theme was added from the repo's history. The picture must be a plain PNG, with no text or other data tucked into it.

Then open a pull request. If anything's wrong, the checks on it will tell you what to fix.

## What we check

The automatic checks run first, on every pull request. They test your folder against the rules below: the file names, the picture's size, the theme's license, every embedded font's license and notices, and that nothing private is in the file.

Then one of us looks at it. We try the theme and watch the art for a while. We might ask for changes, and we might say no.

## Rules

- Only share work you made or have the right to share.
- Don't copy art, logos or characters from games, films or brands. Don't make an "official" look-alike of another product either. A theme inspired by something you love is fine, as long as nothing is copied.
- Embedded fonts must be OFL 1.1 or Apache 2.0. No other font licenses.
- No hidden data. The file should hold the theme and nothing else.
- Art has to stay calm in the middle of the window, where people read. It also has to be light on the computer. Threadlines measures what art costs to draw, and we look at that number.
- Nothing hateful, sexual or harmful.
- We may remove any theme at any time.

## Licenses

Each theme carries its own license in its file, under `credits.license`. It must be `CC-BY-4.0`, so anyone can use it as long as they credit you, or `CC0-1.0`, which gives it away with no conditions.

Fonts keep their own licenses. They must be OFL 1.1 or Apache 2.0, and the font file has to keep its copyright notice and license reference. Fonts from Google Fonts and Bunny Fonts already do. Each theme's `NOTICE.md` lists its credit, its license, and every font's copyright and license. The full license texts are in [`licenses/`](licenses/).

The repo's own files, meaning the workflows and these docs, are MIT. See [LICENSE](LICENSE). That license doesn't cover the themes.

## It's public right away

A pull request is public the moment you open it. Anyone can see the theme, its picture, your credit and your GitHub name. If you chose to include the prompt that made the theme, they can see that too.

Your email isn't shared when you use **Share to Showcase…** in Threadlines after 0.10.0. Version 0.10.0, and a pull request you make by hand, use the email your GitHub account or your git puts on commits.

You can take a share back until it's added. Open the theme's menu in Threadlines and pick **Take back from Showcase…**, or close the pull request yourself. Either way the closed pull request stays on GitHub, so look over what you're sharing before you send it.

## Takedown

If a theme here uses something of yours without permission, [open a takedown request](https://github.com/Threadlines/themes/issues/new?template=takedown.yml). Tell us which theme it is and what's yours. We act quickly on requests from rights holders.
