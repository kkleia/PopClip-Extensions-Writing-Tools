# PopClip Extensions for Writing Tools

**Description**: These three PopClip extensions, implemented using Shortcuts, allow you to conveniently use Writing Tools on non-editable text.

1. **WritingTools**: Inserts non-editable text into a temporary window in the Stickies app and triggers the primary menu of Writing Tools. You can decide which secondary menu to use.
2. **WritingTools.Summary**: Inserts non-editable text into a temporary window in the Stickies app and directly calls the "Summary" secondary menu of Writing Tools for quicker access.
3. **WritingTools.Keypoint**: Inserts non-editable text into a temporary window in the Stickies app and directly calls the "Keypoint" secondary menu of Writing Tools for quicker access.

> **Note**: This plugin is based on the link: [https://forum.popclip.app/t/how-to-access-macos-writing-tools-using-popclip/3004](https://forum.popclip.app/t/how-to-access-macos-writing-tools-using-popclip/3004). If you encounter issues during installation or usage, reading this post may be helpful.

## Prerequisites

1. If you have Xcode Command Line Tools installed:

    ```bash
    brew install cliclick
    ```

    If not, place the `cliclick` file from the project's root directory into the `/usr/local/bin/` folder and grant execution permissions:

    ```bash
    sudo chmod +x /usr/local/bin/cliclick
    ```

    `cliclick` is a command-line tool for moving the mouse pointer.

## Installation Steps

1. **Install the following three shared Shortcuts by clicking the links:**

    - [WritingTools](https://www.icloud.com/shortcuts/1656599033ea40b590ab4f420853ab63)
    - [WritingTools.Keypoint](https://www.icloud.com/shortcuts/55d02e02717b44cd8ea461af47913095)
    - [WritingTools.Summary](https://www.icloud.com/shortcuts/01c94633c5414573956f8a5f7696bcb7)

2. **Assign Keyboard Shortcuts:**

    | Extension                | Menu Title         | Keyboard Shortcut                  |
    |--------------------------|--------------------|------------------------------------|
    | WritingTools.Summary     | Summarize          | Control + Option + Command + S     |
    | WritingTools.Keypoint    | Create Key Points  | Control + Option + Command + K     |

    Additional: If you want to change the default shortcuts, modify the fourth line from the bottom in the AppleScript within Shortcuts:

    ```applescript
    keystroke "s" using {control down, option down, command down}
    ```

3. **Install the PopClip Extension:**

    1. Clone this repository.
    2. Double-click the `.popclipext` plugin files.