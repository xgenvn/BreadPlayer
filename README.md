#Bread Player aka _Macalifa_
A music player with breads and burgers made for the Windows 10 store to replace history.

[![Gitter](https://img.shields.io/gitter/room/nwjs/nw.js.svg?maxAge=2592000)](https://gitter.im/macalifa/Lobby)
###[Screenshots](https://github.com/theweavrs/Macalifa/wiki/Screenshots):
![Imgur](http://i.imgur.com/QBZY1AB.jpg)

###Main Features:
1. Flawlessly plays mp3 audio. (Further format support to be added in due time.)
2. Import Library & Playlists. (other playlist formats e.g. .m3u, .pls etc. will be made available before final release.) 
3. Other basic music player capabilities such as repeat, suffle etc.
4. ID3 Tag Reader

###Alpha Feature-List:
This is the list of all the features that are added and/or yet to be added before first **Alpha** release.
- [x] Improve shuffle
- [ ] Implement History/Recent View
- [x] Playlist creation, import, export and adding songs to playlists. 
- [x] Album View for Library.
- [x] Play song directly when passed as an argument (From Windows Explorer etc.).
- [x] Drag & Drop support.
- [ ] Sorting, filtering, search etc.
- [x] Full library support and features. 
- [x] Implement SettingsView for main features.
- [ ] Show song's properties (ID3 Info).
- [x] Implement basic player functions.
- [ ] Notification when new song starts playing.
- [x] Save `CurrentlyPlayingSong` and info before `ApplicationExit`.
- [x] Support for Windows 10 Mobile

##About the project:
This project is being developed to acknowledge and rectify the scarcity of Music players in Windows 10 Store and also to provide flawless and feature-rich Music player to the end-user. It is still in a very **experimental stage**. [Go here to get an idea of where the project's going.](https://github.com/theweavrs/Macalifa/wiki/Road-to-the-first-release)
###Why the name change?
Basically, the main reason behind the name change is that the previous one didn't make any sense but aside from that it wasn't SEO friendly. Who would _ever_ search for the word _Macalifa_? :D The second reason that is why we chose **Bread Player**, is because it is catchy and it invokes curiousity; furthermore, it has a nice ring to it and it is metaphoric...you know breads and burgers :D
###Main Focus:
Currently the focus is on the **BreadPlayer.Core**, more specifically on the core features such as library/playlist support, bug hunting, basic player capabilites etc. The core focus will be on **performance**, the experience should be as smooth as possible.
###Technologies used:
1. C#/.NET
2. UWP API (Windows Aniversary Edition 10.0; Build 14393)
2. [BASS](http://www.un4seen.com/bass.html) & [ManagedBass](https://github.com/ManagedBass/ManagedBass) (for audio processing)
3. [LiteDB](https://github.com/mbdavid/LiteDB) (for library managment)

###Contributors:
_I am not an expert developer and as a result the code-base isn't as professional as it could be. Hence, I will highly appreciate any contribution in any field regarding this project. All suggestions and issue reporting are welcome._
##Build Notes:
1. Make sure you have the necessary tools for building [Windows Universal Apps](https://dev.windows.com/en-us/develop/building-universal-Windows-apps).
2. Clone this repo:  `git clone https://github.com/theweavrs/Macalifa/`
3. The current version uses the latest Aniversary Edition of UWP (Universal Windows Platform) build 14393 but it is not restricted to that, a lower build version can be used without any problems.
4. ~~To build and debug **Macalifa** flawlessly, the bass.dll must be placed under _Macalifa.Core\bin\PLATFORMVERSION\Debug\Appx_. This problem is currently being acknowledged and fixed. [(Get bass.dll from here.](http://www.un4seen.com/stuff/bass24-winstore.zip) Make sure to use the correct version of bass.dll for the specific platform version (x86\x64\ARM). [For more help go here](http://www.un4seen.com/forum/?topic=16665)).~~ **FIXED [(Issue #4)](https://github.com/theweavrs/Macalifa/issues/4)**
5. ~~"Compile with .NET Native Toolchain" under Build settings of the project must be left unchecked. This is a bug in the _bass.dll_.~~ **FIXED [(Issue #5)](https://github.com/theweavrs/Macalifa/issues/5)**

###NOTE:
_The current **alpha-of-the-alpha** version is under heavy development and will undergo thousands of changes before made available to the end-user._
