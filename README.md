> **Note**: When 'Shortcuts' is used in combination with keyboard shortcuts, it represents a keyboard shortcut. When 'Shortcuts' is used independently, it refers to the Mac application.
# PopClip Extensions for Writing Tools

**Description**: These three PopClip extensions, implemented using Shortcuts, allow you to conveniently use Writing Tools on non-editable text.

1. **WritingTools**: Inserts non-editable text into a temporary window in the Stickies app and triggers the primary menu of Writing Tools. You can then decide which secondary menu to use.
2. **WritingTools.Summary**: Inserts non-editable text into a temporary window in the Stickies app and directly calls the "Summary" secondary menu of Writing Tools for quicker access.
3. **WritingTools.Keypoint**: Inserts non-editable text into a temporary window in the Stickies app and directly calls the "Keypoint" secondary menu of Writing Tools for quicker access.

> **Note**: For installation or usage issues, refer to this [forum post](https://forum.popclip.app/t/how-to-access-macos-writing-tools-using-popclip/3004), It is the source of this plugin.

## Prerequisites

1. If you have Xcode Command Line Tools installed:

    ```bash
    brew install cliclick
    ```

    If Xcode Command Line Tools are not installed, place the `cliclick` file from the project's root directory into `/usr/local/bin/` and grant execution permissions:

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
    
    > **Warning**: Keyboard shortcuts are set in the system settings under App Shortcuts, rather than directly in the Shortcuts editor. If set incorrectly in the Shortcuts editor, it can cause infinite loops and system crashes.

    **Additional**: If you want to change the default shortcuts, modify the fourth line from the bottom in the AppleScript within Shortcuts:
    ```applescript
    keystroke "s" using {control down, option down, command down}
    ```

3. **Install the PopClip Extension:**

    1. Clone this repository.
    2. Double-click the `.popclipext` plugin files.

4. **Permissions and others**

    1. On first use, you need to grant clipboard permissions and Accessibility permissions for `clicclick`, `Stickies`, `Shortcuts`. Select "Always Allow" and "Allow" respectively. These permission requests will automatically pop up the request interface when the plugin is used for the first time.

    2. You can set the font and other settings of Stickies to a comfortable format, and it will use the set format subsequently.

