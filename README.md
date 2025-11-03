# Rate Your Music / Sonemic Tag Hierarchy for MusicBee

A MusicBee tag hierarchy template created as a copy of the Rate Your Music genre and scenes & movements trees.

*This project is unaffiliated with Sonemic.*

[Link to the project on Rate Your Music](https://rateyourmusic.com/list/flaky_bastard/_unofficial-rym-genre-hierarchy-template-for-musicbee/)

## Installation
Firstly, enable the Tag Hierarchy Explorer by going to *View > Arrange Panels* and dragging the Tag Hierarchy Explorer option to one of the available left panes.

Then, simply copy+pasting the contents of the text file into the editor will be enough, which is accessible by going into the Tag Hierarchy Explorer menu and clicking Edit Tag Hierarchy. If you wish not to replace MusicBee's default template or maintain separate tag hierarchy templates, you can drop the text file into MusicBee's TagHierarchyTemplates folder instead.

For those who want to do the latter, quit MusicBee and go to the following folder:

- for those who have installed from the standard installer, go to your `Application Data/Roaming` folder. On Windows, you can paste `%APPDATA%` into Explorer which will drop you into the folder.
- for those who have installed from the Microsoft Store, `AppData\Local\Packages\50072StevenMayall.MusicBee_kcr266et74avj\LocalCache\Roaming\` (thank you RYM user **mallavity**)
- for those who have installed MusicBee in the WINE compatibility layer, find the WINE prefix or "bottle" it was installed in. Then, go to `drive_c/users/YOURUSERHERE/Application Data/Roaming`

Go to the MusicBee folder in Roaming, and a "TagHierarchyTemplates" folder should be available (MusicBee would have made it when the Tag Hierarchy Explorer was enabled). Copy the .txt file to the folder and then restart MusicBee. Your tag hierarchy explorer should have an option titled "RateYourMusic Genre Hierarchy".

## Notes
Since this is all done by hand, some entries might be missing or inaccurate, but it should be accurate from 15th June 2021 onwards, with the intention of regular updates. I also comment on what genres have been changed in every commit, in case people need to update their tags. Report any inaccuracies to either the issues page here, my Rate Your Music account or my socials (see profile)

I have applied for access to RYM's genre dataset, in the hopes I am able to automate this process without accuracy issues in the future.

### Assigning Release Genres ("Entire album")
For assigning genres to entire releases like RYM's release tagging, create a custom tag in MusicBee (Preferences --> Tags (1) --> Define New Tags) then fill your files with the relevant tags in the new custom tag. Then, if you want to use this tag hierarchy for entire releases rather than individual songs, replace album in the hierarchy with the identifier you chose for the release genre tag.
If there's a "standard" custom tag RYM users want to use, I will happily make a template to accomodate this so it's as easy as copy-and-paste/drag-and-drop.

You can also do this to define a separate tag for scenes and movements if you want to use that data as well. I plan to accomodate this use case as long as a custom tag is agreed on - see issue #2.

### Tagging Multiple Genres/Scenes/Movements
RYM allows tagging of multiple genres/scenes/movements for not just a release as a whole, but for individual songs as well. If you intend to follow this while tagging your own library, it's best to use a tagging format capable of storing multiple values in a tag. MusicBee shows this universally by separating tags in its tag editor with a semicolon. I've had someone mention issues with using tag hierarchies with their genre tags, so I thought I'd mention this here.

Vorbis comments (used by FLAC, OGG, Opus and other "Vorbis" codecs) and APE tags are fine, MP3 may need resaving as ID3v2.4 rather than 2.3, MP4/M4A (iTunes store purchases) is notoriously awful and has inconsistent support across multiple players, not just MusicBee - don't use it if you plan to make use of tag hierarchy files.

### "Descriptor" Meta-Genres
RYM allows tagging of descriptors to denote features of the releases documented on their site. Some genres are being moved to the descriptor system (e.g. holiday music, soundtracks, mashup, a cappella) however there has been a freeze on the genre hierarchy, thus no genres can be removed yet without the permission of the moderation team. As a result, genres that are intended to be moved into the descriptor system have been given the Descriptor meta-genre as a parent. The tag hierarchy file maintains this part of RYM's hierarchy but places it in the "Uncategorised" section alongside other uncategorised genres.

## Thanks
- **Londinium** for creating an initial version of the RYM genre tree as a MusicBee tag hierarchy template. If it weren't for them I wouldn't have caught Darkwave years ago.
- Everyone who has reported inaccuracies on the list.
