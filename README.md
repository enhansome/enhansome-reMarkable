# Awesome reMarkable with stars

# [<img src="Awesome.png"></p>](https://github.com/sindresorhus/awesome) ⭐ 501,042 | 🐛 105 | 📅 2026-08-21

The [reMarkable](https://www.remarkable.com) is a paper tablet for those who prefer writing on paper. Its remarkably fast paper-white display, Linux based operating system and awesome community make it highly attractive amongst hackers and developers.

*Contributions are welcome as long as they follow the [guidelines](CONTRIBUTING.md).*

## Disclaimer

No project here is affiliated or endorsed by [reMarkable AS](https://github.com/remarkable). If you modify your device official support might refuse to help you.

### Write down your SSH password

**:warning: WARNING, READ THIS FIRST :warning:**

**Make sure you have saved your SSH password somewhere secure, or you have setup a [SSH key](https://remarkable.guide/guide/access/ssh.html#creating-a-ssh-key)**

You can find the SSH password in your settings: `Settings > Help > Copyrights and licenses > General information (scroll down)`.

Failure to do so could result in a **soft-bricked device** that requires [emergency recovery](https://remarkable.guide/tech/recovery.html).

### Factory reset may brick your device

This function may not do what you are expecting. While it resets all user data, it will not restore the device to the original factory condition. It will reset your SSH password and remove all SSH keys, which may make it impossible to connect to your device if it is malfunctioning.

See [remarkable.guide](https://remarkable.guide/tech/factory-reset.html) for more information on how to properly factory reset your device.

### Take special care if you are using a reMarkable 2.

* System recovery requires some hardware. See <https://remarkable.guide/tech/recovery.html#remarkable-2-recovery> for more information.
* The screen on rm2 and rm1 are different. Workarounds have been developed to interact with the rM2 framebuffer but some projects might not work on it. See [ddvk/remarkable2-framebuffer](https://github.com/ddvk/remarkable2-framebuffer) ⭐ 309 | 🐛 15 | 🌐 C | 📅 2024-10-07 and [ddvk/remarkable2-framebuffer#14](https://github.com/ddvk/remarkable2-framebuffer/issues/14) ⭐ 309 | 🐛 15 | 🌐 C | 📅 2024-10-07.

## Contents

* [APIs](#apis)
  * [Cloud API](#cloud-api)
  * [Lines Format](#lines-format)
  * [Other APIs](#other-apis)
* [Applications](#applications)
  * [Games](#games)
  * [Launchers](#launchers)
* [Cloud Tools](#cloud-tools)
* [Custom Templates](#custom-templates)
* [Device Tools](#device-tools)
* [GUI Clients](#gui-clients)
* [Interface Customization](#interface-customization)
* [Other](#other)
* [Screen Sharing/Streaming](#screen-sharingstreaming)

## APIs

### Cloud API

* [rmfakecloud](https://github.com/ddvk/rmfakecloud) ⭐ 1,324 | 🐛 35 | 🌐 Go | 📅 2026-07-10 - Fake Cloud Sync, server implementation of the Cloud API.
* (Unmaintained) [reMarkableAPI](https://github.com/splitbrain/ReMarkableAPI) ⚠️ Archived - Docs and implementation of the reMarkable file sync API.
* [rMAPI](https://github.com/ddvk/rmapi) ⭐ 310 | 🐛 17 | 🌐 Go | 📅 2026-08-23 ReMarkable Cloud Go API.
* (Unmaintained) [rmapy](https://github.com/subutux/rmapy) ⚠️ Archived - ReMarkable Cloud Python API.
* (Unmaintained) [google-drive-remarkable-sync](https://github.com/bsdz/google-drive-remarkable-sync) ⚠️ Archived - Apps Script API for reMarkable Cloud. Includes Synchronizer capability to automate mirroring of documents from Google Drive to reMarkable Cloud.
* (Unmaintained) [reMarkable-typescript](https://github.com/Ogdentrod/reMarkable-typescript) ⚠️ Archived - TypeScript API for reMarkable Cloud.
* [Remarkable.jl](https://github.com/theogf/Remarkable.jl) ⭐ 40 | 🐛 3 | 🌐 Julia | 📅 2024-02-02 - Julia API Interface to the reMarkable cloud.
* [rmcl](https://github.com/rschroll/rmcl) ⭐ 39 | 🐛 7 | 🌐 Python | 📅 2022-03-30- Asynchronous Python library for the reMarkable Cloud.
* [jrmapi](https://github.com/jlarriba/jrmapi) ⭐ 22 | 🐛 8 | 🌐 Java | 📅 2022-09-27 - A Java API for the reMarkable Cloud.
* [remarkdav](https://github.com/hansegucker/remarkdav) ⭐ 9 | 🐛 5 | 🌐 Python | 📅 2022-09-23 - A tool to sync PDF files from a WebDAV directory to the reMarkable Cloud.

### Lines Format

* [rmscene](https://github.com/ricklupton/rmscene) ⭐ 152 | 🐛 4 | 🌐 Python | 📅 2026-04-05 - Python library to read v6 files / software version 3.
* [rmrl](https://github.com/rschroll/rmrl) ⭐ 139 | 🐛 14 | 🌐 Python | 📅 2021-11-06 - The reMarkable Rendering Library for Python converts annotated documents to PDF files.
* (Unmaintained) [reMarkable-layers](https://github.com/bsdz/remarkable-layers) ⚠️ Archived - Python API for reading & writing reMarkable Lines format. Supports very basic conversion of PDFs and SVGs to Lines format.
* [lines-are-beautiful](https://github.com/ax3l/lines-are-beautiful) ⭐ 112 | 🐛 9 | 🌐 C++ | 📅 2019-11-04 - C++ File API for the reMarkable tablet.
* [lines-are-rusty](https://github.com/ax3l/lines-are-rusty) ⭐ 95 | 🐛 4 | 🌐 Rust | 📅 2021-12-12 - Rust File API for the reMarkable tablet.
* [reMarkable-kaitai](https://github.com/matomatical/reMarkable-kaitai) ⭐ 14 | 🐛 2 | 🌐 Kaitai Struct | 📅 2021-09-19 - [Kaitai Struct](https://kaitai.io/) format specification for the binary lines format.

### Other APIs

* [libreMarkable](https://github.com/canselcik/libremarkable) ⭐ 700 | 🐛 11 | 🌐 C | 📅 2026-06-16 - A framework for developing applications with native refresh support for reMarkable Tablet.

## Applications

* [KOReader](https://github.com/koreader/koreader) ⭐ 29,349 | 🐛 1,327 | 🌐 Lua | 📅 2026-08-29 - An ebook reader application supporting PDF, DjVu, EPUB, FB2 and many more formats.
* [whiteboard-hypercard](https://github.com/fenollp/reMarkable-tools) ⭐ 235 | 🐛 30 | 🌐 Rust | 📅 2026-08-17 - Live collaboration, drawing, chat, whiteboarding.
* [reMarkable keywriter](https://github.com/dps/remarkable-keywriter) ⭐ 227 | 🐛 17 | 🌐 QML | 📅 2024-01-13 - A distraction free keyboard notes app.
* [reMarkable wikipedia](https://github.com/dps/remarkable-wikipedia) ⭐ 174 | 🐛 13 | 🌐 QML | 📅 2022-03-16 - Offline wikipedia reader for reMarkable.
* [darvin/plato](https://github.com/darvin/plato) ⭐ 124 | 🐛 8 | 🌐 Rust | 📅 2019-01-12 [LinusCDE/plato](https://github.com/LinusCDE/plato) ⭐ 53 | 🐛 4 | 🌐 Rust | 📅 2025-09-17 - Plato reader port. Supports pdfs, epubs, many other formats.
* [Rebook](https://github.com/fsniper/ReBook) ⭐ 86 | 🐛 1 | 🌐 C++ | 📅 2023-08-29 - The missing book store for reMarkable.
* [reGenda](https://github.com/tenJirka/reGenda) ⭐ 37 | 🐛 2 | 🌐 Python | 📅 2023-10-20 - An agenda-based calendar for reMarkable.
* (Unmaintained) [remarkaBot](https://github.com/Davide95/remarkaBot) ⚠️ Archived - Fetch your documents from Telegram.
* [Writerdeck for reMarkable 1](https://github.com/bjornte/Writerdeck-for-reMarkable) ⭐ 2 | 🐛 0 | 🌐 Go | 📅 2026-08-22 - Distraction-free Markdown word processor with keyboard support via a companion app or usb. With optional syncing and encryption of documents.
* [harmony](https://rmkit.dev/apps/harmony) - a low latency sketching app with procedural brushes.

### Browser extensions

* [rePub](https://github.com/hafaio/repub) ⭐ 92 | 🐛 2 | 🌐 TypeScript | 📅 2026-08-15 - unofficial browser extension that creates ePubs from websites and can either upload them to reMarkable cloud or save them locally, currently for Chrome only
* [rePubfox](https://github.com/jrockwar/repubfox) ⭐ 23 | 🐛 5 | 🌐 TypeScript | 📅 2024-11-24 - a hard fork of rePub for Firefox

### Games

* [chessMarkable](https://github.com/LinusCDE/chessmarkable) ⭐ 134 | 🐛 3 | 🌐 Rust | 📅 2025-09-16 - Play chess against a bot or a friend.
* [recrossable](https://github.com/sandsmark/recrossable) ⭐ 73 | 🐛 6 | 🌐 C++ | 📅 2021-01-15 - Crossword game with simplistic handwriting recognition and automatic generation of crosswords.
* [DOOMarkable](https://github.com/LinusCDE/doomarkable) ⭐ 51 | 🐛 2 | 🌐 Rust | 📅 2025-09-16 - Play DOOM on the reMarkable 1.
* [retris](https://github.com/LinusCDE/retris) ⭐ 39 | 🐛 0 | 🌐 Rust | 📅 2025-09-16 - Play a clone of the popular block stacking game with either buttons or swipe guestures.
* [minesweeper](https://rmkit.dev/apps/minesweeper) - A mine detection game.

### Launchers

* [draft-reMarkable](https://github.com/dixonary/draft-reMarkable) ⭐ 153 | 🐛 17 | 🌐 C++ | 📅 2022-02-09 - A launcher for the reMarkable tablet, which wraps around the standard interface.
* [oxide](https://oxide.eeems.codes) - A launcher application for the reMarkable tablet.
* [remux](https://rmkit.dev/apps/remux) - A multi-tasking launcher for the reMarkable tablet.

## Cloud Tools

* [remarkable-mcp](https://github.com/SamMorrowDrums/remarkable-mcp) ⭐ 212 | 🐛 8 | 🌐 Python | 📅 2026-08-17 - Model Context Protocol server enabling AI assistants to read and browse your reMarkable documents via SSH (no subscription required) or Cloud API. [Blog post](https://sam-morrow.com/blog/building-an-mcp-server-for-remarkable).
* [reMarkable\_syncthing](http://github.com/evidlo/remarkable_syncthing) ⭐ 210 | 🐛 2 | 📅 2023-07-18 - Syncthing on reMarkable.
* [zotero-reMarkable](https://github.com/michaelmior/zotero-remarkable) ⭐ 191 | 🐛 5 | 🌐 PHP | 📅 2020-06-01 - Script to sync PDFs from the [Zotero](https://www.zotero.org/) reference manager.
* [reGitable](https://github.com/after-eight/regitable) ⭐ 114 | 🐛 5 | 🌐 Shell | 📅 2020-12-23 - Backup your reMarkable with git and sync changes to a remote repository automatically.
* [RMfuse](https://github.com/rschroll/rmfuse) ⭐ 102 | 🐛 22 | 🌐 Python | 📅 2024-04-08 - FUSE filesystem for the reMarkable Cloud.
* [rM-sync](https://github.com/simonschllng/rm-sync) ⭐ 88 | 🐛 6 | 🌐 Shell | 📅 2021-02-26 - Sync script for reMarkable paper tablet.
* [url2epub](https://github.com/fishy/url2epub) ⭐ 82 | 🐛 2 | 🌐 Go | 📅 2026-08-22 - Telegram bot to generate ePub out of URL and send directly to reMarkable Cloud.
* [Moss](https://github.com/RedTTGMoss/moss-desktop) ⭐ 78 | 🐛 6 | 🌐 Python | 📅 2026-08-22 - An app for working with your documents in the reMarkable/rmFakeCloud cloud
* (Unmaintained) [reCatchable](https://github.com/lapwat/reCatchable) ⚠️ Archived - Turn websites into ebooks, upload them to reMarkable.
* [remarking](https://github.com/sabidib/remarking) ⭐ 60 | 🐛 14 | 🌐 Python | 📅 2022-05-29 - CLI tool to extract highlights from any document in the reMarkable cloud.
* [pdf2remarkable](https://github.com/teticio/pdf2remarkable) ⭐ 59 | 🐛 1 | 🌐 Python | 📅 2025-04-02 - Script to upload PDFs to the reMarkable Cloud.
* [Aviary](https://github.com/rmitchellscott/aviary) ⭐ 57 | 🐛 0 | 🌐 Go | 📅 2026-08-26 - A webhook-driven document uploader for reMarkable Cloud and rmfakecloud, featuring a static UI and a Go backend. Optional integration for email via AWS SES.
* [reMarkable-Sink](http://github.com/hmenzagh/reMarkable-Sink) ⭐ 48 | 🐛 0 | 🌐 JavaScript | 📅 2020-11-21 - Turn a folder into a wormhole to your reMarkable.
* [sync\_zotero\_remarkable](https://github.com/danijoo/sync_zotero_remarkable) ⚠️ Archived - Sync PDFs from Zotero to reMarkable.
* [CUPS Printing](https://github.com/ofosos/scratch/tree/master/remarkable-cups) ⭐ 45 | 🐛 5 | 🌐 Python | 📅 2022-06-18 - Script to print directly to reMarkable Cloud from CUPS using rMAPI.
* (Unmaintained) [Zotero2reMarkable Bridge](https://github.com/opal06/zotero2remarkable_bridge) ⚠️ Archived - Sync files from Zotero to reMarkable and back based on tags; supports v2.7< highlights.
* [remarkable-substack](https://github.com/jwoglom/remarkable-substack/) ⭐ 25 | 🐛 2 | 🌐 Python | 📅 2026-07-28 - Syncs unread Substack posts to the reMarkable Cloud.
* [remarkable-zapier](https://github.com/artes-dev/remarkable-zapier) ⭐ 25 | 🐛 3 | 🌐 JavaScript | 📅 2021-04-02 - Zapier Integration for reMarkable Cloud
* [mendeley-rMsync](https://github.com/anilkyelam/mendeley-rMsync) ⭐ 24 | 🐛 4 | 🌐 Python | 📅 2021-09-22 - Script to sync PDFs (with annotations) from/to a [Mendeley](https://www.mendeley.com/) folder.
* [rm-pdf-tools](https://github.com/skius/rm-pdf-tools) ⭐ 21 | 🐛 5 | 🌐 Go | 📅 2021-12-01 - Service that allows users to insert and delete pages from annotated PDFs on the device.
* [reMarkable RSS](https://github.com/eksubin/Remarkable-RSS-Feed) ⭐ 20 | 🐛 0 | 🌐 Python | 📅 2025-08-12 - Read RSS feeds on reMarkable via google drive integration. Automated Script to convert RSS-feeds as PDFs and upload to google drive.
* [AgentNews-RemarkableRSSReader](https://github.com/eksubin/AgentNews-RemarkableRSSReader) ⭐ 15 | 🐛 0 | 🌐 Python | 📅 2025-08-12 - An AI agent for processing RSS news feeds and sending them to reMarkable via Google Drive API.
* [Syncthing-for-reMarkable-AppLoad](https://github.com/paviro/Syncthing-for-reMarkable) ⭐ 13 | 🐛 0 | 🌐 Rust | 📅 2026-06-07 - Syncthing appload app for reMarkable (incl. Paper Pro and Paper Pro Move).
* [remarkable\_simplenote](https://github.com/bgribble/remarkable_simplenote) ⭐ 12 | 🐛 1 | 🌐 Python | 📅 2021-03-06 - Sync simplenote notes to reMarkable (currently one-way)
* [rm-brain](https://github.com/gabrielanhaia/remarkable-brain) ⭐ 9 | 🐛 14 | 🌐 TypeScript | 📅 2026-08-12 - Turns your reMarkable notebooks into a local-first, searchable second brain you query through Claude Desktop.
* [send-to-remarkable](https://github.com/zegevlier/send-to-remarkable) ⭐ 8 | 🐛 5 | 🌐 TypeScript | 📅 2026-04-08 - Upload documents to the reMarkable from an email, like send to Kindle.
* [reMarkable Todoist and Calendar Sync](https://github.com/usuallycwdillon/remarkable-calendar) ⭐ 6 | 🐛 0 | 🌐 Python | 📅 2026-02-02 Puts Todoist tasks and Google calendar events on a calendar then pushes to reMarkable.
* [reMarkable Morning News\_2](https://github.com/ktibr0/Remarkable_morning_news_2) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-07-14 - Automatically sends daily news to your reMarkable tablet. Standalone web application with persistent storage.
* [Remarcal](https://remarcal.com/) - Sync Google, Outlook, Apple, and more calendars to reMarkable.
* [rss2remarkable](https://codeberg.org/akselmo/rss2remarkable) - Generates PDF of given RSS feeds and send is to your reMarkable cloud.

## Custom Templates

* [latex-yearly-planner](https://github.com/kudrykv/latex-yearly-planner) ⭐ 1,525 | 🐛 22 | 🌐 Go | 📅 2026-05-03 - PDF planner designed for e-ink devices.
* (Unmaintained) [ReCalendar](https://github.com/klimeryk/recalendar) ⚠️ Archived - Highly customizable calendar generator in PHP optimized for reMarkable.
* [reMarkable planning/journaling templates](https://github.com/msencer/remarkable_templates) ⭐ 138 | 🐛 0 | 🌐 Makefile | 📅 2024-01-18 - Collection of daily/weekly planning, journaling templates
* [reMarkable-gtd-templates](https://github.com/BartKeulen/remarkable-gtd-templates) ⭐ 85 | 🐛 0 | 🌐 TeX | 📅 2021-09-11 - "Getting Things Done" templates.
* [reMarkable-bujo](https://github.com/vonneudeck/remarkable-bujo) ⭐ 60 | 🐛 0 | 📅 2025-02-20 - "Bullet Journal" templates.
* [rM2Mods templates](https://github.com/DanielRunningen/rM2Mods/tree/main/assests/templates) ⭐ 42 | 🐛 0 | 📅 2025-05-03 - Collection of different templates. E.g., micro dots/grids, checklists, budgeting,  boxes.
* [blank\_slate\_pdf](https://github.com/sowcow/blank_slate_pdf) ⭐ 33 | 🐛 11 | 🌐 Rust | 📅 2026-08-14 - Flexible PDFs for nested lists or experiments with no predefined template, separate simple calendar, customization using ruby code.
* [reMarkable\_templates](https://github.com/steka/reMarkable_templates) ⭐ 22 | 🐛 0 | 📅 2024-03-07 - White lines/squares on gray background.
* [reMarkabletemplates](https://github.com/equivocates/remarkabletemplates/) ⭐ 20 | 🐛 0 | 📅 2024-10-07 - Planner per 1 or 3 weeks.
* [re-Planner](https://github.com/PepikVaio/reMarkable_re-Planner) ⭐ 5 | 🐛 4 | 📅 2025-12-27 - Watermarked PDF calendar for reMarkable 1 and 2. You can pay to remove the watermark, and to receive a customized version.
* [Mobile UX Sketching Templates](https://github.com/Martes-Delta-Co/Remarkable-Mobile-Prototyping-Templates) ⭐ 3 | 🐛 0 | 🌐 Python | 📅 2026-06-10 - Mobile phone templates with 12 column layouts, grids, and multiple combinations of 1/2/4-up layouts with space for note-taking, in iPhone and Android flavors, in Methods format, so you can swap templates on each page of a notebook
* [remarkable-engineering](https://gitlab.com/asciipip/remarkable-engineering) - Engineering-style grid templates.

### Template Builders

* [Daily Journal / Wardley Maps / Figma template](https://www.figma.com/community/file/1389237140795352688) - A daily planner/journal, Wardley Map, and forkable general starter kit for building custom templates with Figma.
* [ReCalendar.me](https://recalendar.me/) - Highly customizable online calendar generator optimized for reMarkable.
* [Remarkable Grid Template Generator](https://xosh.org/remarkable-grid-template/) - Generate pixel perfect line grid and dotted grid templates
* [Remarkably Planner Builder](https://remarkably-organized.pages.dev/) - Generate hyperlinked pdf planners
* [reMarkable Template Builder](https://templarian.github.io/remarkable/) - Generate Isometric and Grid templates of all sizes

## Device Tools

* [rm-version-switcher](https://github.com/rmitchellscott/rm-version-switcher) ⭐ 21 | 🐛 1 | 🌐 Go | 📅 2026-05-11 - An interactive CLI application for switching between installed reMarkable OS versions.
* [paginator](https://github.com/aflusche/paginator) ⭐ 18 | 🐛 1 | 🌐 C++ | 📅 2024-03-11 - Physical foot pedal to turn pages on the device with no hands (e.g. for playing sheet music).
* (Unmaintained)[remarvin](https://github.com/plan5/remarvin) ⭐ 8 | 🐛 5 | 🌐 Shell | 📅 2024-04-16 - Profile and file encryption manager that allows to manage notebooks for different users and to optionally protect the files with a password through gocryptfs-based encryption (device only).
* [rmtree](https://github.com/rmitchellscott/rmtree) ⭐ 6 | 🐛 1 | 🌐 Go | 📅 2026-07-02 - Unix-style tree command for the reMarkable's document filesystem.
* [reExecute](https://github.com/Slenderman00/reExecute) ⭐ 2 | 🐛 0 | 🌐 Shell | 📅 2026-05-08 - Persistent code execution bootstrap for reMarkable Paper Pro Move using the MDM agent config.
* [rmtemplate](https://github.com/zer0trip/rmtemplate) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-07-21 - CLI to upload and manage custom templates on reMarkable Paper Pro and Paper Pro Move devices over SSH.
* [splash.dat converter](https://gist.github.com/iTrooz/fddfcce03c1c44b04231be73d6e7982a) - Simple script to convert an image to the rM2 .dat format for a splash screen.

## GUI Clients

* [reManager](https://github.com/rmitchellscott/reManager) ⭐ 349 | 🐛 8 | 🌐 TypeScript | 📅 2026-08-27 - Linux, MacOS, and Windows desktop app for managing mods on reMarkable tablets using the [Vellum](https://github.com/vellum-dev/vellum) ⭐ 121 | 🐛 7 | 🌐 Shell | 📅 2026-08-27 package manager.
* [ReMy](https://github.com/bordaigorl/remy) ⭐ 310 | 🐛 25 | 🌐 Python | 📅 2025-05-11 - A GUI to browse, preview documents, export documents with custom settings, all via SSH (no cloud needed); works from local raw backups too.
* [RemaPy](https://github.com/peerdavid/remapy) ⭐ 182 | 🐛 12 | 🌐 Python | 📅 2022-07-29 - GUI to browse, download/upload files and backup the tablet (also on Linux) using the cloud.
* [reMarkable-assistant](https://github.com/richeymichael/remarkable-assistant) ⭐ 180 | 🐛 16 | 🌐 Python | 📅 2021-05-29 - Manage templates, splash screens, and settings on your reMarkable tablet.
* (Unmaintained) [Slithin](https://github.com/furesoft/Slithin) ⚠️ Archived - Free Management Application for Windows/Linux/MacOS.
* [reMarkable-hyutilities](https://github.com/moovida/remarkable-hyutilities) ⭐ 85 | 🐛 6 | 🌐 Java | 📅 2023-04-14 - A GUI written in java to backup your device, upload templates and modify splash screens.
* [rMExplorer](https://github.com/bruot/pyrmexplorer/wiki) ⭐ 73 | 🐛 9 | 🌐 Python | 📅 2021-09-11 - GUI to browse, download/upload files and backup the tablet without using the cloud.
* [rmUploader](https://github.com/lobre/rmuploader) ⭐ 60 | 🐛 5 | 🌐 Go | 📅 2020-02-23 - Simple web app to upload epub or pdf files to the reMarkable tablet via drag and drop.
* [reMarkable Remember](https://github.com/ds160/remarkable-remember) ⭐ 56 | 🐛 0 | 🌐 C# | 📅 2026-07-14 - A cross-platform client for offline management of backups, notebooks, templates and hand writing recognition via MyScript.
* [asTounding](https://github.com/jlarriba/astounding) ⭐ 50 | 🐛 5 | 🌐 Java | 📅 2022-01-04 -  A multiplatform GUI application for the reMarkable cloud, including Linux.
* [rm-exporter](https://github.com/chopikus/rm-exporter) ⭐ 46 | 🐛 2 | 🌐 Go | 📅 2026-01-07 - Exports any combination of folders and large notes locally, supports Windows/MacOS/Linux.
* [RMHook](https://github.com/NohamR/RMHook) ⭐ 9 | 🐛 2 | 🌐 C++ | 📅 2026-08-27 - A dynamic library injection tool for the reMarkable Desktop macOS application, enabling connection to self-hosted rmfakecloud servers.
* [RMHook-Win](https://github.com/NohamR/RMHook-Win) ⭐ 4 | 🐛 0 | 🌐 C++ | 📅 2026-08-25 - A hooking tool for the reMarkable Desktop Windows application, enabling connection to self-hosted rmfakecloud servers.
* [RMHook-iOS](https://github.com/NohamR/RMHook-iOS/) ⭐ 0 | 🐛 1 | 🌐 Logos | 📅 2026-08-27 - A hooking tool for the reMarkable iOS application, enabling connection to self-hosted rmfakecloud servers.
* [reMarkable Connection Utility (RCU)](http://www.davisr.me/projects/rcu/) - Cross-platform local/offline client for managing backups, screenshots, notebooks, templates, wallpaper, firmware, and third-party software. Typed text and snap highlight extraction. Virtual printer for native print-to-tablet.
* [rM2 Template Helper](https://www.freeremarkabletools.com/) Windows tool for template management, and to download community templates.

## Interface Customization

* [rM Hacks](https://github.com/mb1986/rm-hacks) ⭐ 662 | 🐛 166 | 🌐 Shell | 📅 2024-06-11 - Small improvements and tweaks for rM devices.
* [RemarkableLamyEraser](https://github.com/isaacwisdom/RemarkableLamyEraser/) ⭐ 305 | 🐛 3 | 🌐 C | 📅 2025-02-02 - Supports Lamy Al Star stylus button to erase or undo for reMarkable tablets.
* [rM Hacks (QLMDiff)](https://github.com/asivery/rm-hacks-qmd) ⭐ 230 | 🐛 11 | 📅 2026-04-08 - Port of rmhacks for xovi.
* [ReCept](https://github.com/funkey/recept/) ⭐ 172 | 🐛 12 | 🌐 C++ | 📅 2023-05-04 - Fix for the rM2 jagged line issue.
* [rm-xovi-extensions](https://github.com/asivery/rm-xovi-extensions) ⭐ 130 | 🐛 1 | 🌐 C | 📅 2026-05-23 - extensions for the reMarkable tablets, which utilize the xovi framework
  * `framebuffer-spy` - Exposes the address of the system framebuffer.
  * `qt-command-executor` - Injects a Qt module to execute shell commands from QML.
  * `qt-resource-rebuilder` - Injects into Qt and rebuilds resource databases on the fly, allowing QML/image replacement or addition.
  * `random-suspend-screen` - Randomize your reMarkable tablet's suspend screens.
  * `webserver-remote` - Exposes the USB webserver to all interfaces, with a confirmation dialog for inbound connections.
* [AppLoad](https://github.com/asivery/rm-appload) ⭐ 95 | 🐛 11 | 🌐 C++ | 📅 2026-08-26 - Enables windowed and fullscreen apps inside the reMarkable interface.
* [xovi-extensions (FouzR)](https://github.com/FouzR/xovi-extensions) ⭐ 90 | 🐛 2 | 📅 2026-08-23
  * `favTagButton` - Adds quick access buttons for Favourites and Tagged files.
  * `floating` - Adds a floating toolbar.
  * `gestures` - Adds several useful gestures.
  * `recentsTagged` - New menu showing tagged files, sorted by last modified.
  * `selectionErase` - Enables deleting a stroke via selection tool.
  * `selectionStuff` - Adds "select everything above the line."
* [Crazy Cow](https://github.com/machinelevel/sp425-crazy-cow) ⭐ 88 | 🐛 11 | 🌐 C++ | 📅 2021-09-15 - Typewriter input from USB keyboard directly into reMarkable interface.
* [WebInterface-OnBoot](https://github.com/rM-self-serve/webinterface-onboot) ⭐ 45 | 🐛 5 | 🌐 Shell | 📅 2024-08-18 - Enable the web interface on boot.
* [WebInterface-Wifi](https://github.com/rM-self-serve/webinterface-wifi) ⭐ 43 | 🐛 4 | 🌐 Rust | 📅 2025-02-04 - View the web interface if running, over wifi.
* [xovi-tripletap](https://github.com/rmitchellscott/xovi-tripletap) ⭐ 37 | 🐛 1 | 🌐 Shell | 📅 2026-05-12 - Start xovi with a triple-press of the power button.
* [xovi-qmd-extensions (ingatellent)](https://github.com/ingatellent/xovi-qmd-extensions) ⭐ 29 | 🐛 1 | 🌐 QML | 📅 2026-07-23
  * `changeVerticalJump` - Increase page scroll distance.
  * `delayStrokeRefresh` - Delay refresh after a colored stroke.
  * `enableAllColors` - Enable full color palette on greyscale devices.
  * `enableExtraPenOnMove` - Adds an extra pen slot to the toolbar
  * `enableShortcuts` - Add keyboard shortcuts for navigation.
  * `enableShortcutsWithScrollOrChangePage` - Adds keyboard shortcuts when used with gestures.
  * `feverLightSteps` - Change brightness slider behavior from 5 to 4 levels.
  * `gestures` - Gestures for zoom, toolbar toggle, navigation, contrast filter.
  * `hideDocumentClose` - Hide the close button in documents.
  * `hidePageLabelsInFullscreen` - Hide page numbers at the bottom of the screen when the toolbar is hidden.
  * `hideShowToolbar` - Hide the button for showing/hiding the toolbar.
  * `miniLightSleep` - Show a line of text at the bottom right corner instead of the light sleep banner.
* [xovi-qmd-extensions (rmitchellscott)](https://github.com/rmitchellscott/xovi-qmd-extensions) ⭐ 29 | 🐛 3 | 🌐 Shell | 📅 2026-08-28
  * `createPagesPaperProSize` - Override new page creation to use Paper Pro dimensions.
  * `createPagesRM2Size` - Override new page creation to use reMarkable 2 dimensions.
  * `disableSelectionAutoScroll` - Disable auto scrolling when moving a selection.
  * `hideDevModeIcon` - Hide the developer mode icon next to the battery icon.
  * `hideZoomIndicator` - Auto-hide zoom indicator after 4 seconds.
  * `miniLightSleep` - Replaces the light sleep banner with text saying "Sleeping" with a white background at the top right of the screen.
  * `preventNotebookZoomOut` - Forces all notebook pages to start at 1x zoom with optional horizontal offset. Designed for the Paper Pro Move.
  * `quickSettingsScreenshot` - Adds a screenshot button to the quick settings menu.
  * `unlockMethodsContent` - Bypass subscription check for using on-device Methods templates and documents.
* [rM-signature-patch](https://github.com/Barabazs/rM-signature-patch) ⭐ 22 | 🐛 0 | 🌐 Shell | 📅 2024-03-29 - Simple script to remove that pesky advert at the bottom of a mail originating from a reMarkable.
* [reLuminate](https://github.com/unreMarkableLabs/reLuminate) ⭐ 16 | 🐛 1 | 🌐 Shell | 📅 2025-12-02 - Enable enhanced screen brightness levels on the reMarkable Paper Pro.
* [WebInterface-Upload-Button](https://github.com/rM-self-serve/webinterface-upload-button) ⭐ 12 | 🐛 1 | 🌐 JavaScript | 📅 2024-07-01 - Upload button for the web interface, alternative to drag and drop.
* [xovi-qmd-extensions (StarNumber12046)](https://github.com/StarNumber12046/xovi-qmd-extensions) ⭐ 12 | 🐛 2 | 📅 2025-12-30
  * `autoNewPage` - Removes the "New Page" button when swiping past end.
  * `clock` - Adds a sidebar clock.
  * `hideDocumentClose` - Removes document close button.
  * `hideShowToolbar` - Hides the "Show Toolbar" button.
  * `miniLightSleep` - Replaces light sleep banner with "Zzz…" text.
  * `pagesIndicator` - Displays page count in sidebar.
  * `quickSettingsClock` - Adds a clock to the quick settings menu.
  * `thickness` - Adds more pen thickness options.
  * `uncompressCreate` - Expands "+" menu with separate folder/notebook/page options.
* [Book-safe](https://github.com/dvdsk/Book-safe) ⭐ 8 | 🐛 12 | 🌐 Rust | 📅 2026-07-23 - Hide books/documents between a given time period.
* [remarkable-shortcuts](https://github.com/martinetd/remarkable-shortcuts) ⭐ 8 | 🐛 1 | 🌐 Python | 📅 2023-05-16 - Add extra 'gestures' (currently double taps) for easier navigation.
* [Signature-rM](https://github.com/rM-self-serve/signature-rM) ⭐ 6 | 🐛 1 | 🌐 Rust | 📅 2024-03-14 - Remove the signature from the bottom of emails sent from the device.
* [xovi-qmd-extensions (NohamR)](https://github.com/NohamR/xovi-qmd-extensions) ⭐ 6 | 🐛 0 | 🌐 Shell | 📅 2026-07-17
  * `clock` - Adds a live clock to the library sidebar; tap the entry to toggle seconds display.
  * `convertToText_remover` - Removes the Convert to text option from selection menus and the toolbar.
  * `favoriteButton` - Restores a Favorite action in the document list header for faster pinning.
  * `forceSync` - Adds a cloud button in Quick Settings that forces a library sync when tapped.
  * `hideDocumentClose` - Hides the close button in the document toolbar to prevent accidental exits.
  * `quickSettingsClock` - Injects a tappable clock into the Quick Settings header; tap to toggle between minute and second.
  * `tagButton` - Puts a Tag action next to other list controls to open the tag editor directly.
  * `uncompressDock` - Replaces the condensed More menu in the new document dock with dedicated buttons for notebook, folder, and quick sheet creation.
* [rm-hacks-xovi-qmd (Samarkin)](https://github.com/Samarkin/rm-hacks-xovi-qmd) ⭐ 4 | 🐛 0 | 📅 2026-08-16
  * `clearScreenBeforeLocking` - Fixes ghosting when using custom suspend screen.
  * `enableExtraPenOnMove` - Adds a slot for the second pen on Paper Pro Move.
  * `eraseSelection` - Adds an option to delete selection without losing clipboard contents.
  * `forceRefreshGesture` - Adds a gesture to force refresh the screen to eliminate accumulated ghosting.
  * `frontLightIcon` - Adds a front light status indicator to document mode.
  * `gestures` - Adds gestures to switch between two pens and selection tool without the need to show toolbar.
  * `hideCloseButton` - Hides the close button in document view to allow for more space on Paper Pro Move.
  * `instantFavorites` - Removes the delayed refresh of document drawer at the cost of not showing the latest list.
  * `toolbarIcon` - Modifies the show toolbar button to display color of the current tool.
  * `uncompressDock` - Replaces the '+' button in the navigator view with the actual icons.
* [webinterface-rmpp](https://github.com/t3rminalV/webinterface-rmpp) ⭐ 0 | 🐛 0 | 🌐 Shell | 📅 2026-06-04 - Enable web interface on boot and over wifi on the reMarkable Paper Pro. Includes authentication and SSL.

## Other

* [reMarkable\_mouse](https://github.com/evidlo/remarkable_mouse) ⭐ 633 | 🐛 28 | 🌐 Python | 📅 2026-08-15 - Use your reMarkable as a graphics tablet.
* [paper2reMarkable](https://github.com/GjjvdBurg/paper2remarkable) ⭐ 384 | 🐛 7 | 🌐 Python | 📅 2025-02-16 - Download an academic paper or HTML article, crop it, and send it to the reMarkable with a single command.
* [Goosepaper](https://github.com/j6k4m8/goosepaper) ⭐ 343 | 🐛 20 | 🌐 Python | 📅 2026-08-18: Deliver prettily-formatted RSS feeds, news articles, Wikipedia articles-of-the-day, and more to your reMarkable tablet.
* [remarkable\_news](https://github.com/evidlo/remarkable_news) ⭐ 299 | 🐛 4 | 🌐 Go | 📅 2026-04-08 - Use daily news/comics/images as the suspend screen.
* [remarkable\_printer](https://github.com/Evidlo/remarkable_printer) ⭐ 299 | 🐛 6 | 🌐 Go | 📅 2026-03-30 - Print from any device to reMarkable without browser extensions or reMarkable cloud.
* [reMouseable](https://github.com/kevinconway/remouseable) ⭐ 251 | 🐛 9 | 🌐 C | 📅 2024-09-20 - Use your reMarkable tablet as a mouse.
* (Unmaintained) [reHackable/scripts](https://github.com/reHackable/scripts) ⚠️ Archived - A set of bash scripts that may enhance your reMarkable experience.
* [morningpaper2reMarkable](https://github.com/jessfraz/morningpaper2remarkable) ⭐ 231 | 🐛 4 | 🌐 Go | 📅 2023-02-23 - A bot to sync the morning paper to a reMarkable tablet.
* [pocket2rm](https://github.com/glidergeek/pocket2rm) ⭐ 193 | 🐛 12 | 🌐 Go | 📅 2023-02-01 - Synchronize articles from read-later platform pocket in PDF and epub.
* [reMarkable\_entware](http://github.com/evidlo/remarkable_entware) ⭐ 193 | 🐛 6 | 🌐 Shell | 📅 2024-12-27 - Package manager for reMarkable.  Install common Unix utilities through the command line.
* [reMarkableSync](https://github.com/jamesf91/reMarkableSync) ⭐ 178 | 🐛 23 | 🌐 C# | 📅 2024-11-09 - A Microsoft OneNote addin for importing notebooks from reMarkable as text or images.
* [reHackable/maxio](https://github.com/reHackable/maxio) ⭐ 166 | 🐛 21 | 🌐 Shell | 📅 2022-05-05 - Companion daemon for the reMarkable paper tablet.
* [reMarkablePocket](https://github.com/nov1n/RemarkablePocket) ⭐ 163 | 🐛 0 | 🌐 Java | 📅 2025-05-19 - Synchronize articles from read-later platform Pocket in epub format.
* [remailable](https://github.com/j6k4m8/remailable) ⭐ 139 | 🐛 16 | 🌐 Python | 📅 2021-12-23 - Email PDFs directly to your reMarkable. ([Free publicly-hosted version available](https://remailable.getneutrality.org/)).
* [rmirro](https://github.com/hersle/rmirro) ⭐ 125 | 🐛 7 | 🌐 Python | 📅 2025-01-12 - A script that synchronizes PDFs of documents between a Remarkable and a computer folder that mirrors its file structure without cloud access.
* [rMsync](https://github.com/lschwetlick/rMsync) ⭐ 99 | 🐛 3 | 🌐 Jupyter Notebook | 📅 2022-05-06 - Synchronisation script with a local dedicated "library" folder.
* [reMarkable CLI tooling](https://github.com/cherti/remarkable-cli-tooling) ⭐ 95 | 🐛 2 | 🌐 Python | 📅 2024-02-19 - CLI-tooling to sync documents to a reMarkable, to clean deleted files etc. without needing cloud access
* [reMarkable\_pdflets](https://github.com/evidlo/remarkable_pdflets) ⭐ 93 | 🐛 0 | 🌐 Shell | 📅 2021-02-26 - Dynamically updating PDFs.
* (Unmaintained) [Calibre-Remarkable-Device-Driver-Plugin](https://github.com/naclander/Calibre-Remarkable-Device-Driver-Plugin) ⚠️ Archived - A Calibre Plugin to Manage your Remarkable Books.
* [reMarkable-fs](https://github.com/nick8325/remarkable-fs) ⭐ 87 | 🐛 14 | 🌐 Python | 📅 2022-04-05 - A FUSE filesystem wrapper for the reMarkable tablet.
* [rM-dl-annotated](https://github.com/jmptable/rm-dl-annotated) ⭐ 84 | 🐛 3 | 🌐 Shell | 📅 2020-10-04 - Export annotated PDFs from reMarkable tablets.
* [reSnap](https://github.com/cloudsftp/reSnap) ⭐ 80 | 🐛 4 | 🌐 Shell | 📅 2026-08-20 - Take snapshots of your reMarkable screen over SSH.
* [reMarkable-touchgestures](https://github.com/ddvk/remarkable-touchgestures) ⭐ 70 | 🐛 2 | 🌐 C | 📅 2020-12-21 - Touch gestures (swipe/touch) for easy page navigation.
* [pdf2rmnotebook](https://github.com/JCN-9000/pdf2rmnotebook) ⭐ 66 | 🐛 6 | 🌐 Shell | 📅 2026-01-31 - Creates a reMarkable Notebook from multiple PDF files.
* [rmWacomToMouse](https://github.com/LinusCDE/rmWacomToMouse) ⭐ 64 | 🐛 0 | 🌐 Python | 📅 2021-11-17 - Use the wacom pen as a mouse to draw on your pc.
* [remarks](https://github.com/Scrybbling-together/remarks) ⭐ 63 | 🐛 20 | 🌐 Python | 📅 2026-08-27 - Extract highlights, scribbles, and annotations from PDFs. Export to Markdown, PNG, and SVG.
* [Epistolary](https://github.com/j6k4m8/epistolary) ⭐ 62 | 🐛 2 | 🌐 Python | 📅 2025-02-06 - Emails on the reMarkable. Read and respond to your email inbox in handwriting (auto-converts to text before sending).
* [Ephemeris](https://github.com/rmitchellscott/ephemeris) ⭐ 54 | 🐛 1 | 🌐 Python | 📅 2026-07-31 - A Python-based tool that generates clean, daily schedules using ICS calendar data. Designed with e-ink tablets like reMarkable in mind.
* [nix-remarkable](https://github.com/siraben/nix-remarkable) ⭐ 54 | 🐛 1 | 🌐 Nix | 📅 2026-05-16 - Nix expressions for the reMarkable tablet leveraging the company's toolchain.
* [instapaper-as-pdf-to-reMarkable](https://github.com/fabianmu/instapaper-as-pdf-to-remarkable) ⭐ 45 | 🐛 2 | 🌐 JavaScript | 📅 2018-03-18 - Export Instapaper-Articles to PDF and send them to a connected rM tablet.
* [reMarkable-random-screens](https://github.com/Neurone/reMarkable) ⭐ 44 | 🐛 0 | 🌐 Shell | 📅 2023-06-20 - Change your poweroff and suspend screens every 5 minutes with random images of your choice
* [rmWebUiTools](https://github.com/LinusCDE/rmWebUiTools) ⭐ 42 | 🐛 6 | 🌐 Python | 📅 2024-08-04 - View a file tree, see statistics and export/backup all files with some simple scripts utilizing the web ui.
* [reMarkable\_keyboard](https://github.com/Evidlo/remarkable_keyboard) ⭐ 39 | 🐛 2 | 🌐 Python | 📅 2024-02-14 - Software to use rM as wireless keyboard/mouse.
* [rmTabletDriver](https://github.com/LinusCDE/rmTabletDriver) ⭐ 31 | 🐛 0 | 🌐 C | 📅 2020-01-28 - Application that allows you to simulate/clone rM input on your computer.
* [landscape-pdf](https://github.com/nmoran/landscape-pdf) ⭐ 28 | 🐛 2 | 🌐 Python | 📅 2021-01-07 - Utility to convert pdf documents to read in landscape mode. Useful for papers and text books.
* [Funcky reMarkable Exporter](https://github.com/simonbaudart/Funcky.Remarkable.Exporter) ⭐ 25 | 🐛 0 | 🌐 C# | 📅 2018-07-20 - Export notes from a reMarkable Tablet to File System and External Services.
* [RMPP Entware](https://github.com/hmenzagh/rmpp-entware) ⭐ 25 | 🐛 1 | 🌐 Shell | 📅 2026-03-24 - Package manager for reMarkable Paper Pro.  Install okpg package manager.
* (Unmaintained) [reMarkable-tweak](https://github.com/morngrar/remarkable-tweak) ⚠️ Archived - Tweak tool for the reMarkable paper tablet. Lets you organize your templates with no fuss.
* [reMarkable-crosswords](https://github.com/shapeshed/remarkable-crosswords) ⭐ 24 | 🐛 1 | 🌐 Shell | 📅 2023-03-07 - Get crosswords freshly delivered to your Remarkable every morning.
* [reMarkable-tablet-driver](https://github.com/FreeCap23/reMarkable-tablet-driver) ⚠️ Archived - Use your reMarkable as a drawing tablet in Linux with pressure sensitivity and tilt. Works in Wayland.
* [send\_by\_rmapi](https://github.com/LisaGlaser/send_by_rmapi) ⭐ 15 | 🐛 0 | 🌐 Python | 📅 2023-08-02 - A Calibre plugin to send books to your reMarkable, making use of rmapi.
* [rm2anki](https://github.com/stelzch/rm2anki) ⭐ 14 | 🐛 0 | 🌐 Rust | 📅 2024-01-14 - Convert reMarkable notebooks into an Anki card decks.
* [ePUB to reMarkable PDF](https://github.com/suntorytimed/epub_to_remarkable) ⭐ 12 | 🐛 1 | 🌐 Python | 📅 2025-04-01 - Self hostable web service for turning an EPUB into a reMarkable optimised PDF.
* [mail2rm](https://github.com/glatzor/mail2rm) ⭐ 10 | 🐛 3 | 🌐 Python | 📅 2021-05-03 - Mail PDF documents to your reMarkable cloud using your mail transport agent e.g. postfix.
* [rmathlab](https://github.com/Samdney/rmathlab) ⭐ 9 | 🐛 0 | 🌐 Python | 📅 2025-03-07 - A Linux toolset for the reMarkable 2 tablet, which enables math handwriting recognition and LaTeX generation over USB via Mathpix.
* [neofetch](https://github.com/rM-self-serve/neofetch-rM) ⭐ 8 | 🐛 0 | 🌐 Shell | 📅 2024-03-14 - A command-line system information tool written in bash 3.2+.
* [rm-pySAS](https://github.com/tenJirka/rm-pySAS) ⭐ 7 | 🐛 0 | 🌐 Python | 📅 2023-08-25 - Python wrapper for [simple](https://rmkit.dev/apps/sas).
* [remarkable-ssh](https://github.com/Penguin-Guru/remarkable-ssh) ⭐ 6 | 🐛 0 | 🌐 Shell | 📅 2026-03-05 - A bash script to manage files on reMarkable devices via CLI and SSH.
* [remarkable-nixos](https://github.com/gitman-101111/remarkable-nixos) ⭐ 3 | 🐛 0 | 🌐 Nix | 📅 2026-07-28 - Run NixOS on your reMarkable Pro Paper Move (others possible)
* [remarkable-api](https://github.com/Penguin-Guru/remarkable-api) ⭐ 2 | 🐛 1 | 🌐 Shell | 📅 2026-02-19 - A simple bash script to interact with reMarkable devices' USB Web Interface.
* [chiappa](https://github.com/gitman-101111/chiappa) ⭐ 1 | 🐛 0 | 🌐 C | 📅 2026-07-28 - e-Ink bridge/miscellaneous scripts and tools to port other OS's to a reMarkable Pro Paper Move.
* [reCalibre-Driver](https://github.com/zer0trip/reCalibre) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2026-07-27 - A Calibre plugin for syncing books to a reMarkable, via KOReader or the native UI.
* [Drawj2d](https://drawj2d.sourceforge.io/) - Create technical line drawings on an editable reMarkable notebook page. ([Guidance how to upload](https://sourceforge.net/p/drawj2d/wiki/reMarkable/) the page to the device using rMAPI.)
* [microSD](http://www.davisr.me/projects/remarkable-microsd/) - Tutorial for adding a microSD card reader to the reMarkable 1.
* [Parabola-rM](http://www.davisr.me/projects/parabola-rm/) - A Desktop GNU/Linux-libre replacement OS with fast partial refreshing and USB OTG.
* [remt](https://gitlab.com/wrobell/remt) - reMarkable tablet command-line tools.

## Screen Sharing/Streaming

* [reStream](https://github.com/rien/reStream) ⭐ 865 | 🐛 10 | 🌐 Shell | 📅 2026-06-10 - Stream your reMarkable screen over SSH.
* [rMview](https://github.com/bordaigorl/rmview) ⭐ 829 | 🐛 47 | 🌐 Python | 📅 2025-10-08 - A fast GUI to stream your reMarkable screen over vanilla-SSH or VNC.
* [goMarkableStream](https://github.com/owulveryck/goMarkableStream) ⭐ 748 | 🐛 26 | 🌐 Go | 📅 2026-08-21 - Stream the screen of the reMarkable 2 (FW 2.5) easily (client/server in Go with no installation) along with the colors (with FW > 2.11.x).
* [VNSee](https://github.com/matteodelabre/vnsee) ⭐ 300 | 🐛 24 | 🌐 C++ | 📅 2021-08-29 - VNC client for the reMarkable tablet allowing you to use the device as a second screen.
* [srvfb](https://github.com/merovius/srvfb) ⭐ 246 | 🐛 8 | 🌐 Go | 📅 2023-10-03 - Alternative screen-streaming software. Written in Go.
* [rM-vnc-server](https://github.com/peter-sa/rM-vnc-server) ⭐ 88 | 🐛 9 | 🌐 C | 📅 2021-07-06 - A fast & efficient damage-tracking (sending only updated regions) VNC server for streaming the reMarkable's screen.
* [pipes and rust](https://github.com/AnyTimeTraveler/pipes-and-rust) ⭐ 66 | 🐛 4 | 🌐 HTML | 📅 2021-12-04 - (Made for rM2) Stream pen strokes to browser. A single executable on the reMarkable that hosts a tiny webserver in the local WLAN.
* [pipes and paper enhanced](https://github.com/Pyrrhu5/pipes-and-paper-enhanced/tree/stable) ⭐ 56 | 🐛 2 | 🌐 Python | 📅 2025-06-06 - Share the pen strokes to a browser without installling anything on the ReMarkable (a revived fork of the previous link with pen colors and eraser support, responsive interface).
* [AppLoad-RMStream](https://github.com/asivery/appload-rmstream) ⭐ 13 | 🐛 2 | 🌐 Rust | 📅 2026-05-26 - An AppLoad application for streaming your reMarkable tablet's screen over HTTP.
* [pipes and paper](https://gitlab.com/afandian/pipes-and-paper) - Stream pen strokes to browser canvas via websockets ([blog post](https://blog.afandian.com/2020/10/pipes-and-paper-remarkable/)). Uses Python and SSH, nothing to compile or install on the reMarkable device.

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-29._
