# Explorer Tab Memory Saver

A Windhawk mod that remembers the tabs in the last File Explorer window you close. Reopen Explorer to **Home** or **This PC** to return to the folder you were using. Open a specific folder and it stays selected while the saved folders reopen as tabs in the same window.

By [Maxxwell Quinn](https://github.com/MXXQN). Tested on Windows 11 x64, build 26300.9974, with native File Explorer tabs.

The similarly named [Explorer Tabs Session Saver](https://windhawk.net/mods/explorer-tabs-session-saver) opens saved folders through the Windows shell and recommends a companion utility to group them into tabs. Explorer Tab Memory Saver creates native tabs directly in the window you open and restores the selected folder. It works with Windhawk alone.

## Install manually

1. Open the [mod source](explorer-tab-memory.wh.cpp) and copy the entire file.
2. In Windhawk, open **Home** and select **Create a New Mod**. If you already use a local copy of Explorer Tab Memory, open that mod in the editor to update it.
3. Replace the editor contents with the copied source, then select **Compile Mod**.
4. Check that **Explorer Tab Memory Saver** is enabled. To try it, open two folders in separate tabs, close the last Explorer window, and reopen Explorer.

## What gets saved

The mod saves the folder paths and active tab for the last window you close. Duplicate tabs are preserved. Windows supplies the tab order, which can differ from an order you set by dragging tabs.

Each Windows user has a separate session in `HKEY_CURRENT_USER\Software\ExplorerTabMemory`. Leave the **Windows account SID** setting empty to enable the mod for all users, or enter a user’s SID to restrict it to that account.

[Source repository](https://github.com/MXXQN/explorer-tab-memory-saver) · [MIT license](LICENSE)
