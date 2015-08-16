JSPlaylist
a jscript for foobar2000 panel "WSH Panel Mod 1.5.6"
----------------------------------------------------
coded by Br3tt (http://br3tt.deviantart.com)

// [Features]
// * Groups (collpase or expand, add extra lines, ...)
// * Custom Group By patterns with Playlist Filter feature like in ELPlaylist
// * Custom Panel Colors
// * Smooth Scrolling
// * Arrange columns as you want, create custom columns with titleformatting and specific color
// * Playlist Header at Top (can be disabled)
// * Wallpaper as background supported (including a new blur effect)
// * Playlist Manager collapsable panel
// * Built in Settings Panel (still some minor parameter to edit in Properties of the panel)
// * Sort by clicking column header
// * Windows scaling compliant (dpi)
// * Playback statistics Engine (update file tags, now asynchronously on tracks ending)
// * ... and more!
//[/Features]
//
// [Requirements]
// * foobar2000 v1.1 or better >> http://www.foobar2000.org
// * WSH panel Mod v1.5.6 or better >> http://code.google.com/p/foo-wsh-panel-mod/downloads/list
// * Windows fonts : WingDings 1, 2 & 3
// [/Requirements]
//
// [Options]
// * Font guifx v2 transports >> http://blog.guifx.com/2009/04/02/guifx-v2-transport-font
// [/Options]
//
// [Installation]
// * disable "Safe Mode" option in WSH Panel Mod preferences (menu File>Preferences>Tools>WSH Panel Mod)
// * copy "wsh_br3tt" folder into your foobar2000 Profile folder (it only contains the jsplaylist subfolder)
// * import/paste the main JSPlaylist script into a WSH Panel Mod instance of your foobar2000 layout (DUI or CUI)
// * Important: for any Y major update of my scripts (where Y is 2nd number version => x.Y.z), replace the whole folder "wsh_br3tt\jsplaylist\" each time
//   and Clear the WSH panel properties (hold SHIFT key + Right-click > Properties > "Clear" button > "OK" button)
// [/Installation]
//
// [Tips]
// * Hold SHIFT key + right click on a toolbar to display Configure script ans panel Properties entries
// * Use Jscript9 engine (if supported by your system) for better performances (known issue: high %cpu on mouse move with older Windows 8.0 versions, in this case prefer Jscript engine)
// * Change colors and fonts in foobar2000 Preferences > DefaultUI or ColumsUI
// * Some minor settings can be changed in window Properties (right click on a playlist item > Settings...), use it carefully! main settings are now built in the panel with a graphic interface
// * Left click on a column header to sort the playlist on this field
// * Right click on the columns toolbar to edit Columns and Groups layout and features
// * Use Keyboard for searching artist in the playlist (incremental search feature like in ELPlaylist) or to navigate in playlist
// * Right Click on items for contextual menu for the selection
// * TAB key or Middle Click to toggle the Playlist Manager
// * CTRL+T to toggle the columns toolbar
// * CTRL+I to toggle the top Info panel
// * Hold CTRL + Mouse Wheel to scale elements (useful for 'retina' screens)
// * F2 key to rename active playlist in playlist manager panel
// * F5 key to refresh covers
// * Special fields handled in columns TF: %list_index%, %list_total%, %isplaying%
// * Special TF function to set specific color for the text that follows it: $rgb(r,g,b) with r,g,b as decimal values [0;255]
//   do not use $rgb(,r,g,b) in a test condition compare but always for the result part (then or else):
//   ==> avoid this: $if($rgb(0,0,0)%title%,%title%,,)
//   ==> but do this: $if(%title%,$rgb(0,0,0)%title%,,)
// * Playlist Filter Groups pattenrs: Set a group by pattern to a playlist thru Groups settings tab or by rigth clicking playlist manager item
// * ... etc
// [/Tips]

feedback is always welcome :)

---
Br3tt