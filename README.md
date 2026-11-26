# Winamp Access

An NVDA add-on that makes Winamp easier to use with NVDA.

**Download:** get the latest `WinampAccess-1.0.nvda-addon` from the [Releases page](https://github.com/ykhandoo108/WinampAccess/releases), open it, and follow NVDA's prompts.

**Requirements:** NVDA 2021.1 or later, and Winamp. Last tested with NVDA 2026.3.1. The optional tempo control also needs the free [Bookamp](https://github.com/michaldziwisz/bookamp) plugin.

**Questions, bug reports and ideas:** use the [Issues](https://github.com/ykhandoo108/WinampAccess/issues) tab, or press Alt+Enter in Winamp to write to the developer.

The full user guide follows. It is also built into the add-on as its help file.

---

Version 1.0

Winamp Access makes Winamp easier to use with NVDA. It offers slider position reporting, better manipulation of sliders, and useful presets for volume, pan, equalizer, preamp and audio tempo controls.

It integrates with the Bookamp plugin to change tempo of media files quickly and provides number-row speed presets for the tempo slider. Bookamp is a free plugin that is installed separately.

In the Playlist editor, it improves track selection and track reordering feedback.

It provides a simple but powerful bookmark system for naming and remembering seeked positions in media files, to return to later. A bookmark can also remember the file it was made in, and load that file again when we go to it. Bookmarks can be imported and selectively or collectively exported to file.

It includes our Winamp Access Settings menu where we can decide how much speech feedback is important, or when confirmations matter when our presets set the volume to maximum or mute, or maximize, minimize or flatten the preamp and the Equalizer bands.

We keep many well-known shortcuts from older JAWS scripts for Winamp and from the ExtendedWinamp add-on, to promote a familiar feel to long-time Winamp users. Winamp Access builds on these older foundations. To our knowledge, no earlier NVDA add-on or JAWS script for Winamp has combined all of the following in one place: spoken volume and panning reports, preset slider positions for volume, panning, the preamp and every equalizer band, tempo control through Bookamp with speed presets, a detailed bookmark manager, and a settings dialog for choosing how much is spoken or confirmed.

With this Winamp Access add-on, NVDA's input help, NVDA+1, we now announce most of Winamp's most used native keyboard commands.

In Winamp, Control Tab natively navigates us between the main window, playlist editor and equalizer. The Winamp Access scripts now speak each of these windows clearly as they land.

## Requirements

Winamp Access works with NVDA 2021.1 or later. It was last tested with NVDA 2026.3.1.

## Installing

Open the add-on file, follow NVDA's prompts, and restart NVDA when asked.

Two Winamp add-ons cannot work together, so before installing, Winamp Access looks for any other installed add-on that has to do with Winamp. If it finds one, it names it and asks whether to uninstall it. Choose Yes only if you want the extended accessibility features of Winamp Access instead.

- **Yes**: that add-on is scheduled for removal and Winamp Access is installed. Both take effect when NVDA restarts.
- **No**, or the other add-on cannot be uninstalled from here: nothing is installed and nothing is changed. You are told which add-on to remove yourself. Open the NVDA menu, then Tools, then Add-on Store (or Manage add-ons in older NVDA versions), select it, choose Remove, restart NVDA, and open the Winamp Access file again.

Installing a newer version of Winamp Access over an older one is a normal update.

## Uninstalling

Our bookmarks and Winamp Access settings are saved in NVDA's user configuration folder, outside the add-on itself. The bookmarks are in the file WinampAccess.wab, and the settings are in the WinampAccess section of nvda.ini and of any NVDA configuration profile that has them. When Winamp Access is removed from NVDA's Tools menu, Add-on Store, NVDA asks us to restart. NVDA completes the removal while it is starting, when it cannot yet show or speak a question, so Winamp Access waits until NVDA has finished starting. A few seconds after that, we are asked two questions, one about removing our bookmarks file, and one about removing our saved Winamp Access settings, including the Shift J jump time and the Control R end of track review time. Answering Yes to the settings question removes them from nvda.ini and from every configuration profile. Answering No to either keeps it, for the next time Winamp Access is installed. If NVDA is closed before the questions appear, or they cannot be shown for any reason, nothing is deleted. If we update to a newer version of Winamp Access, nothing is removed and we are not asked.

## Keys that operate from all Winamp windows

- **Play or pause**: Space bar
- **Write to the developer**: Alt Enter
- **Help file**: Question mark
- **Winamp Access Settings dialog**: Control F12
- **Winamp Access Bookmarks manager**: Control Shift B

Notes: The Space bar does the same as Winamp's own C key, which plays or pauses. If Winamp is stopped, Space starts playing, and Winamp's own C key does not.

### Write to the developer with Alt Enter

Press Alt Enter in any Winamp window and Winamp Access starts an E-mail to the developer, Yamuna Jivana Dasa, at <ykhandoo@gmail.com>, with the subject "Winamp Access Support" already filled in. It asks you to confirm first, with OK and Cancel. If you have more than one E-mail program, you are asked which one to use. Web browsers are left out of that list. The developer's address is also copied to the clipboard, and NVDA tells you so. If no E-mail program can be found, NVDA says so and offers to open Gmail in your web browser, with the message already addressed. You can also write to ykhandoo@gmail.com yourself, from any E-mail program you like.

You do not need a problem to write to us. A friendly hello is the best E-mail we can get. Tell us how you use Winamp, what you like listening to, which feature you enjoy most, or what you would love to see added. One line is plenty. "Hi, it works and I like it" tells us this add-on has found a good home, and that makes our day.

Mail is answered in the author's spare time, a resource rarer than a quiet playlist at a party. Replies are expected within two weeks at most. Any delay is honestly regretted, and will be accompanied by tea, guilt and a sincere apology.

## The Winamp Access Settings dialog

The Winamp Access Settings dialog offers us choices for the way we would like to hear spoken feedback or for receiving confirmations for potentially undesirable actions. There is a group for each of these: Volume and panning, Preamp and equalizer, Aggressive changes to sound, Tempo control help and preset names, Bookmarks, and Bookmarks and the playlist. The dialog is opened with Control F12 from any Winamp window and takes the focus when it opens. Our choices are saved in NVDA's configuration, in the WinampAccess section of nvda.ini, together with the jump time set with Shift J and the end of track review time set with Control R. These will be described along with the relevant features throughout this help file.

## Keys that operate from the main window only

- **Activate tempo control**: Shift Up arrow
- **Deactivate tempo control**: Shift Down arrow

Notes: These Winamp Access functions allow us to activate or turn off changing the speed of the audio file by manipulating Winamp's interface, to and from the Bookamp plugin automatically for us. More about this later.

## Keys that operate from the main window and the playlist editor window

- **Report total time of audio file**: Control Shift T
- **Report remaining time of audio file**: Control Shift R
- **Report elapsed time of audio file**: Control Shift E
- **Seek to near end of file**: Shift R
- **Customize distance in seconds for the seek to near end of file**: Control R

Notes: These two commands help with quickly reviewing the end of a media file with ease. Press Control R and specify how many seconds before the end of the file we wish to review. Then press Shift R to automatically have Winamp Access navigate backward from the end of file to that distance, and play that final bit of media to review. The number of seconds in Control R is remembered across sessions.

- **Specify in seconds Custom Seek distances**: Shift J

Notes: This Shift J function exists because Winamp Access provides Control Left arrow and Control Right arrow as custom seek controls for backward and forward respectively. This is in addition to the default 5 seconds seeking provided natively in Winamp using left and right arrows. So the Shift J command allows us to specify the amount for the custom seek in seconds, which determines how much the Control Left and Control Right arrows will seek back and forward through the file. Its value is remembered across Winamp sessions.

## Volume

In the main window and the Equalizer window, Winamp Access provides further functionality to Winamp's own keyboard controls as follows. Winamp natively provides down and up arrows for adjusting the output volume. Winamp Access now provides spoken feedback of the volume control in percentage from mute (0%) to maximum (100%), as you move the volume slider. This can be turned off from the Control F12 Winamp Access settings menu, from the Volume and panning group settings.

We also provide useful volume presets:

- **Home** and **End** keys shoot the volume control to maximum and mute respectively. Because these are aggressive changes to the sound, we are first asked to confirm, and we answer with Enter to proceed or Escape to cancel. If the volume is already at maximum or mute, nothing is asked. These confirmations can be turned off from the Control F12 settings menu, from the Aggressive changes to sound group settings.
- **Page Up** and **Page Down** keys change the volume in 20% increments at a time.
- **Alt Home** sets the volume to 50%, the halfway mark.

## The Winamp Equalizer window

In the equalizer window, left and right arrows natively pan the signal left and right respectively. Winamp Access now announces the percentage left, right, and center as we move the slider. Winamp Access also provides panning presets from all Winamp windows so we don't have to go to the Equalizer window to pan the signal:

- **Control Alt H** and **Control Alt Semicolon** pan the signal completely left and right respectively.
- **Control Alt J** and **Control Alt L** pan the signal 50% left and 50% right respectively.
- **Control Alt K** pans the signal dead center.

For small steps, we can also pan from the main window and the playlist editor with **Shift Left arrow** and **Shift Right arrow**. Each press pans a little further left or right, and Winamp Access announces the position, in the same way as in the Equalizer window. The panning stops at the far left or far right instead of going round.

These are reported by Winamp Access and the reporting can be turned off from the Control F12 settings menu, Volume and panning group, so that panning happens silently.

Winamp Access also provides keyboard functions for manipulating and reporting the preamp volume and the entire ten-band graphic equalizer.

Natively in Winamp, from the top number row of the keyboard, we use the grave accent key to increase the Preamp volume, and we use numbers 1 to 0 to increase each of the ten bands of the graphic equalizer, where 1 deals with the lowest, all the way to 0, the highest frequency band. From the row just below the numbers row, we use the corresponding keys to decrease. So, the Tab key decreases the Preamp volume, while Q through P decrease each of the ten bands of the equalizer, again from the lowest frequency band to the highest respectively.

Winamp Access is now able to report as we adjust the Preamp and each equalizer band's level by telling us which band we are changing, and its value. For example: Preamp is -1.5, Band 1 is 12.0, Band 9 is 8.1, and so on.

We can turn off this reporting of the Equalizer controls, by using the Control F12 settings of Winamp Access, from the Preamp and equalizer group of controls, if this level of feedback is not desired.

If we add the shift key to each of the Preamp and Equalizer increase controls, grave accent to 0, this will shoot the controls to their maximum values, and if we add shift to each of the corresponding keys below, from Tab to P, this will drop them to their minimum values. In each case, for these maximum and minimum jumps, we are asked to confirm, and we answer with Enter to proceed or Escape to cancel. These confirmations can also be turned off from the Control F12 settings menu, from the Aggressive changes to sound group settings, which governs the Home and End volume presets as well as the preamp and equalizer jumps.

Using Control Shift with each of the preamp and Equalizer bands from the number row reports their existing levels without changing those values, useful for confirming levels without making changes.

Using Control Shift with each of the Equalizer band reduction keys from Q to P reports each of their frequencies, so we have an idea of which aspect of the sound spectrum that band will affect. This is purely informational since Winamp uses preset frequencies for each band that cannot be changed, as is standard for a normal audio playback software.

If we use the Alt key alone with each of the band increase controls 1 through 0, this will flatten the bands. Alt Grave accent flattens the Preamp. The confirmations for these can also be turned off from Winamp Access's Control F12 settings menu, from the Aggressive changes to sound group.

## The Playlist editor

Adding files to play in Winamp is easiest done from File Explorer, from the context menu of the media file, Show More options, Play in Winamp, or Enqueue in Winamp.

Once we have built up a list of media files to play, they show up in the Playlist editor. Winamp Access now reads them with up and down arrows. It identifies if the media file is the current track, reads the track name and says its length.

We can reorder the tracks in the Playlist editor by holding the Alt key down on a particular media item, then pressing up or down arrows. This will move the selected item up or down in the list, and Winamp Access will announce its new position out of the total number of positions or total media items.

### Making selections

Since Winamp allows us to add as many contiguous items to the selection as the length of the Playlist editor window, Winamp Access makes the Playlist editor as tall as the screen allows when it gains focus with Control Tab, and puts it back to its normal size when we leave it.

Due to limitations in the Winamp playlist editor, we are unable to make noncontiguous item selections.

Pressing Shift while moving up or down selects the item in that direction, and Winamp Access says Selected, followed by the item and the total number of items selected. If the selection shrinks, it says Unselected, followed by the item that was left out and the total number of items selected. Control A selects every item, and Winamp Access says how many are selected.

If we have made multiple selections this way, we can also then use the Alt key to move our selection up or down with arrows in the Playlist editor as a group.

## Bookmarks

Winamp Access lets us store positions in time, with a name of our choosing, and return to them later. A bookmark is a name, a position in minutes and seconds, and the file that was playing when we made it. Two options on each bookmark decide whether that file is used when we go to the bookmark and when we move it, as described below. Press Control Shift B from any Winamp window to open the Bookmarks manager. It works while Winamp is playing or paused. The Bookmarks window comes to the front of Winamp as it opens, so it never waits unnoticed in the background, and the list has the focus.

The bookmarks are kept in an ordinary text file called WinampAccess.wab, which stands for Winamp Access Bookmark, in NVDA's user configuration folder. Each bookmark takes three lines. The first has the name, a space, the grave accent, a space, and then the position, for example: Chapter 3 \` 1050:25. Because of this, the grave accent cannot be used in a bookmark name. Names can hold letters, numbers, spaces, punctuation, brackets, dashes and the underscore, and are limited to 245 characters so that this line never goes over one line. The second line has the full path of the file in quotation marks, after the word File, for example: File: "X:\Music\Albums\Track 11.wav". The third line has the state of the two options, Yes for checked and No for unchecked, for example: Include file when going to bookmark: Yes, Include file when moving bookmark to new position: Yes. If WinampAccess.wab does not exist when we open the manager, it is created for us.

If the file is not in the format described here, we are told that the bookmark file seems to be corrupt and asked whether to create a new one. Yes deletes the old file and all its bookmarks, and this cannot be reversed. No closes the manager and returns us to Winamp.

We land on a multi-selection list of the bookmark names. As we move through it, Winamp Access speaks the name, then the position of that bookmark. Shift with the arrows selects contiguous bookmarks. Control with the arrows, Home, End, Page up and Page down moves without changing the selection, and Control Space selects or deselects the bookmark we are on. Winamp Access reports the selection as we go. While moving with Control held down, we hear "Selected" or "Unselected", then the bookmark's name, then how many bookmarks are selected in all. Pressing Space with Control held down says "Selected" or "Unselected", then how many bookmarks are selected. Moving with Shift held down says "Selected" before each bookmark that joins the selection, and "Unselected" before a bookmark that leaves it as we go back over it, followed in each case by the number selected. Control A selects all the bookmarks.

To change the order of our bookmarks, select one or more of them in the list and press **Alt Up arrow** to move them up one place, or **Alt Down arrow** to move them down one place. Winamp Access changes the order in WinampAccess.wab first, then updates the list, and reports the new position or positions. If the selection cannot go any further, we are told it is already at the top or at the bottom. Selected bookmarks that are not next to each other all move together.

When a new bookmark is added, the cursor returns to the list, on the new bookmark, which is selected. After the list come these buttons:

- **Go to bookmark**: Seeks Winamp to the bookmark and closes the manager. Enter in the list does the same. It is available only while exactly one bookmark is selected. If Winamp is stopped, playback is started first so that there is something to seek in, and then Winamp seeks to the bookmark. Afterwards Winamp plays on, or is left paused, according to the Bookmarks group in the Control F12 settings, which offers Play media after the Go to bookmark button is pressed, the default, or Pause media after the Go to bookmark button is pressed. If the bookmark has Include file when going to bookmark checked, the file recorded for it is loaded first. What happens to the playlist depends on the Bookmarks and the playlist group in the Control F12 settings, which offers Do not keep previous playlist when going to a bookmark, or Keep previous playlist when going to a bookmark, the default. When we keep the playlist, Winamp Access uses the file if it is already in the playlist, and adds it to the end of the playlist if it is not. When we do not keep it, the playlist is emptied and the file becomes the only item in it, unless it already is. The playlist is never emptied for a file that cannot be found. The playlist is only touched when the bookmark has a file recorded, so a bookmark with Include file when going to bookmark unchecked leaves it alone. If the file cannot be found, we are asked File not found. Move within existing file anyway? Yes seeks to the position in the track that is current, and No returns us to the list with nothing done.
- **Move bookmark to new position**: Replaces the position of the selected bookmark with where Winamp is now, and says, for example, "Chapter 3 moved to 12 minutes, 5 seconds". If the bookmark has Include file when moving bookmark to new position checked, the full path of the file now playing is recorded with it as well.
- **Edit bookmark**: Opens the bookmark's name in an edit field for us to change, with its two checkboxes, Include file when going to bookmark and Include file when moving bookmark to new position, set as they were saved. Ok saves the new name and checkboxes, and also records Winamp's current position and the file now playing for the bookmark. Cancel changes nothing. If nothing is playing in Winamp, the name and checkboxes are saved and the position and file stay as they were. A name already used by another bookmark is refused. F2 in the list does the same. It is available only while exactly one bookmark is selected.
- **Delete selected Bookmarks**: Deletes every selected bookmark. Delete in the list does the same. To delete more than one, first select them in the list, with Shift and the arrows for bookmarks next to each other, or by holding Control, moving with the arrows and pressing Space for bookmarks that are not.
- **Add bookmark**: Asks for a name, with the two checkboxes Include file when going to bookmark and Include file when moving bookmark to new position, which are checked unless we change them. When we press Ok, Winamp's current position and the file now playing are recorded for it, with the state of the checkboxes. If the name already exists, we are told so and returned to the edit field to type another.
- **Import Bookmark file**: Opens a file dialog that shows only .wab files. A file that does not follow the format is refused. We are then asked whether to import into the existing bookmarks, which may leave duplicates, or to import as a new file, which replaces all existing bookmarks.
- **Export bookmark file**: Saves a copy of all our bookmarks, by default as WinampAccess.wab, wherever we choose.
- **Export selected bookmarks to file**: Saves only the selected bookmarks. Select them in the list first. It is available only while something is selected.
- **Close**: Returns to Winamp.

Move, Edit, Delete and the two Export selected functions are also unavailable while there is nothing to act on, so Tab skips them.

## Tempo control

Winamp Access requires that Bookamp is installed to use the tempo functions. While Bookamp allows us to change pitch and speed independently or together (tape style), all accessibly through sliders, Winamp Access focuses on its tempo control, which we find will probably be mainly used for listening to things like audio books at faster speeds.

The tempo functions of Winamp Access operate from Winamp's main window. We activate the tempo function with Shift Up Arrow and deactivate it with Shift Down Arrow. If we press either of these keys while Bookamp is not installed, Winamp Access asks whether we would like to install it now, and we are told that the tempo control needs the free Bookamp plugin. The buttons are Open download page and Cancel. Open download page takes us to Bookamp's download page in our web browser, and Cancel leaves things as they are.

When we activate the tempo function with Shift Up Arrow, Winamp Access says Please wait for speed plugin to activate, activates Bookamp, selects the correct speed algorithm and places us in the Tempo slider. We change the tempo with arrow keys for small speed changes and Page Up and Page Down keys for larger speed changes to the audio.

Winamp Access also provides presets on the number row of the keyboard to change the tempo to precise speeds against the original media. These presets only function in the Bookamp window, while we are navigating the tempo slider. Winamp Access says nothing while the slider moves, then announces the name of the speed once it has settled. The presets are as follows:

- **1**: Half speed.
- **2**: Three quarter speed.
- **3**: Less than normal speed.
- **4**: Normal speed.
- **5**: One and a quarter speed.
- **6**: One and a half speed.
- **7**: One and three quarter speed.
- **8**: Double speed.

Press the Question mark key to hear these presets spoken in that window. This always speaks, even if we have turned the tempo help off. If we choose Do not speak tempo control help or preset names, from the Tempo control help and preset names group of the Control F12 settings, the number keys still set the speed, but silently.

After making our selection, press Alt F4 to close the Bookamp window. We return to Winamp's main window with the new tempo now operating.

If we wish to deactivate Bookamp, we use Winamp Access's Shift Down Arrow to accomplish this most effectively. Winamp Access says Please wait for speed plugin to deactivate, then Shift Down Arrow automates the following:

- Takes us to Winamp's Preferences window,
- turns off Bookamp's DSP effect by changing Winamp's DSP to None,
- changes back to the Output in the preferences menu so that the output plugin has the main focus in preferences,
- and finally closes the Preferences window, returning us to Winamp's main window.

Winamp Access then announces to us that the tempo control is disabled.

I hope Winamp Access Add-on proves useful to you. Shoot us an E-mail with Alt Enter from the Winamp window to say hi and send some feedback.

Regards,

Yamuna Jivana Dasa

## License

Winamp Access is by Yamuna Jivana Dasa. It is free software, covered by the GNU General Public License, version 2 (GPL-2.0). The full text is in the [LICENSE file](https://github.com/ykhandoo108/WinampAccess/blob/main/LICENSE) of the project's source code repository at [github.com/ykhandoo108/WinampAccess](https://github.com/ykhandoo108/WinampAccess).

## Credits

Winamp Access takes some of its keyboard commands from older JAWS scripts for Winamp and from the ExtendedWinamp add-on by Hrvoje Katic, Beka Gozalishvili and the NVDA add-on team, which is itself based on NVDA's own Winamp support by the NVDA Contributors. Our thanks to all of them.

Tempo control works through the Bookamp plugin, which is by its own author: [github.com/michaldziwisz/bookamp](https://github.com/michaldziwisz/bookamp).

## Change log

### Version 1.0

First release.
