<h1 align="center">
  <br>
  <a href="http://github.com/"><img src="https://i.imgur.com/81bz9Ws.png" alt="Cookunity Engineering Team" width="250"></a>
  <br>
Boosting VS Code Efficiency<br>
</h1>
<div align="center">
  :computer:
</div>
<div align="center">
  Interesting <code>tools</code> and <code>tweks</code> using VS Code.
</div>

<br />

<div align="center">
  <sub>Shared by
  <a href="https://www.cookunity.com">
  Cookunity Engineering Team
  </a>
</div>


## Table of Contents

- [Shortcuts](#shortcuts)
- [Configs](#configs)
- [Tips](#tips)
- [Usefull Extension](#usefull-extension)

## Shortcuts

### Standard Shortcuts

| Key Combination           | Action                                                  |
| ------------------------- | ------------------------------------------------------- |
| CMD B                     | Open/Close the sidebar                                  |
| CMD P                     | Open/Close the file switcher                            |
| CMD SHIFT P               | Open/Close the command palette                          |
| `CTL + \`                 | Open/Close the terminal                                 |
| CTL + J                   | Open/Close the panel                                    |
| OPT + DOWN + ,            | Move Line                                               |
| OPT + SHIFT + DOWN + ,    | Duplicate Line                                          |
| OPT + CMD + K + ,         | Duplicate Line                                          |
| CTRL + -                  | Navigate back                                           |
| CTRL + SHIFT + -          | Navigate forward                                        |
| CMD + /                   | Comment line                                            |
| CMD + SHIFT + L           | Add multiple cursors on every selected match            |
| CMD + D                   | Add multiple cursors at a time (for skip, use CMD + K ) |
| OPT + ENTER               | Add multiple cursors when using find box                |
| CMD + P + P               | Switch file                                             |
| CMD + 0                   | Switch to sidebar                                       |
| CMD + 1                   | Switch editor                                           |
| CTRL +                    | Open terminal                                           |
| F2                        | Rename refactor                                         |
| F8                        | Move between errors                                     |
| F5                        | Open debugger                                           |
| CMD .                     | Expand bulb options                                     |
| CMD SHIFT B               | Build process                                           |
| SHIFT + CTL + Right Arrow | Extend selection                                        |

### Custom Shortcuts

| Key Combination | Action              |
| --------------- | ------------------- |
| OPT + CMD + ,   | Open settings UI    |
| OPT + B         | Toggle Activity bar |

## Configs

### Disable Minimap

1. Open Command Palette ( CMD + SHIFT + P on macOS, CTRL + SHIFT + P on Windows/Linux).
2. Type Preferences: Open Settings (UI) and select it.
3. Search for "Minimap" in the search bar.
4. Uncheck the checkbox for "Editor: Minimap" to disable the minimap.

### Toggle Primary Sidebar Position

1. Open Command Palette.
2. Type View: Toggle Side Bar Position and select it to toggle the sidebar position between left and right.

### Disable Open Editors Visible

1. Go to Settings UI as before.
2. Search for "Open Editors".
3. Uncheck the checkbox for "Explorer: Open Editors Visible" to hide the Open Editors pane in the sidebar.

### Settings Editor: JSON

To default to using the JSON editor for settings:

1. Open Command Palette.
2. Type Preferences: Open Settings (JSON) and select it. This will open your settings.json file directly in the future, you can navigate to Preferences: Open Settings (UI) and search for "workbench > settings: Editor" and select "json" from the dropdown.

### Add OPT + CMD + , to Open Normal UI (Settings UI uses AI)

To create a custom keyboard shortcut for opening the Settings UI:

1. Open Command Palette.
2. Type Preferences: Open Keyboard Shortcuts (JSON) and select it.
3. Add the following JSON object to your keybindings file:
   ```json
   {
     "key": "opt+cmd+,",
     "command": "workbench.action.openSettings",
     "when": "settingsEditor:useSplitJSON !== true"
   }
   ```
4. Save the file.

### Disable the Breadcrumbs

1. Open Settings UI.
2. Search for "Breadcrumbs".
3. Uncheck the checkbox for "Breadcrumbs: Enabled" to disable the breadcrumbs feature.

### Toggle Activity Bar OPT + B

To create a custom keyboard shortcut for toggling the Activity Bar:

1. Open Keyboard Shortcuts (JSON) as before.
2. Add the following JSON object to your keybindings file:

```json
{
  "key": "opt+b",
  "command": "workbench.action.toggleActivityBarVisibility"
}
```

3. Save the file.

## Tips

### Search

When using the file switcher:

```
@ symbol browser
@: group symbols
#: search across files for symbol
```

You can use the VS CODE type check withot configure TS
` "js/ts.implicitProjectConfig.checkJs": true`

Logpoints
Console log statements from the editor
![alt text](image.png)

exclude files from the editor

```json
files.exclude
```

### Region folding

This will collapse all the code between these tags

```
// # region Description
// # endregion
```

### Launch config

Use launch config for debugging

Debugger auto-attach
`node --inspect index.js`

## Usefull Extension

### Themes and Icons

- [**Hyper Theme**](https://marketplace.visualstudio.com/items?itemName=jack-curtis.hyper)
- [**Material Icon Theme**](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)

### Workspace Enhancement

- [**Peacock**](https://marketplace.visualstudio.com/items?itemName=johnpapa.vscode-peacock)

### Code Versioning and Management

- [**Version Lens**](https://marketplace.visualstudio.com/items?itemName=pflannery.vscode-versionlens)
- [**GitLens — Git supercharged**](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
- [**GitLab Workflow**](https://marketplace.visualstudio.com/items?itemName=GitLab.gitlab-workflow)

### Development and Programming

- [**Simple React Snippets**](https://marketplace.visualstudio.com/items?itemName=burkeholland.simple-react-snippets)
- [**Docker**](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker)
- [**Docker Explorer**](https://marketplace.visualstudio.com/items?itemName=formulahendry.docker-explorer)
- [**Remote Development**](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)
- [**SQL Notebook**](https://marketplace.visualstudio.com/items?itemName=cmoog.sqlnotebook)
- [**AWS Toolkit**](https://marketplace.visualstudio.com/items?itemName=AmazonWebServices.aws-toolkit-vscode)
- [**GitHub Copilot**](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot)

### Code Formatting and Linting

- [**Prettier - Code formatter**](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

### Collaboration and Project Management

- [**Jira and Bitbucket (Atlassian Labs)**](https://marketplace.visualstudio.com/items?itemName=Atlassian.atlascode)
- [**Live Share**](https://marketplace.visualstudio.com/items?itemName=MS-vsliveshare.vsliveshare)

### Miscellaneous Tools and Enhancements

- [**Annotator**](https://marketplace.visualstudio.com/items?itemName=ryu1kn.annotator)
- [**Better Comments**](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments)
- [**Bookmarks**](https://marketplace.visualstudio.com/items?itemName=alefragnani.Bookmarks)
- [**Code Runner**](https://marketplace.visualstudio.com/items?itemName=formulahendry.code-runner)
- [**Code Spell Checker**](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker) -[**Spanish - Code Spell Checker**](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker-spanish)
- [**GitBook**](https://marketplace.visualstudio.com/items?itemName=GitBook.gitbook-vscode)
- [**Datadog**](https://marketplace.visualstudio.com/items?itemName=Datadog.datadog-vscode)
