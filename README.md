# Photograph-Sorter---lightweight-
Offline, single-file photo organiser with metadata rules, duplicate review, animated sorting, local folder output and ZIP export.

---

## Photo Sorter

An offline photo organiser with a slightly overenthusiastic filing machine.

Photo Sorter is a single-file browser application for sorting photographs, videos and other selected files. I built it to deal with untidy collections without uploading anything or installing a full desktop file manager.

Open the HTML file in a compatible browser, choose some files and press GO. Photographs tumble into their suggested categories while the organiser shows you what it intends to do.

The animation is a preview. Files only change when you separately approve a copy or move, or export an organised ZIP.

### Features

Visual sorting: Animated category trays, a GO button and replay, with a reduced-motion option.

Local metadata reader: EXIF, IPTC and XMP information, including capture dates, camera details, descriptions and supported keywords.

Sorting rules: Combine filenames, metadata, file types and dates. Inspect and adjust decisions before committing them.

Organisation profiles: Save and import or export rules as JSON.

Folder layouts: Organise by category, date, camera or photographic event, with custom destinations where supported.

Duplicate review: SHA-256 checks for identical files and perceptual comparisons to suggest visually similar photographs.

Contact sheet and timeline: Browse thumbnails, review metadata and group photographs into sessions.

Output options: Create organised folders through supported browser file APIs, or export the folder structure as a ZIP.

Recovery tools: Operation receipts, recovery journals and undo support for eligible direct file operations.

Everything runs locally. There are no accounts, external JavaScript libraries or cloud uploads.

### Getting started

Download photo-sorter-v1.1.2-go.html from the project releases or repository and open it in a recent Chromium-based browser. You can also rename it index.html.

Select Demo to explore the interface, or use Choose files or Choose folder to load your collection.

Press GO to run the animated sorting preview.

Open Review classifications to check destinations, edit categories, inspect metadata or adjust your rules.

Use Export ZIP to download organised copies, or Organise files to copy or move them to a chosen destination where your browser supports direct folder access.

Start with a disposable folder. Check the output before allowing the application to move anything important.

### How sorting works

The organiser considers file types, filenames, embedded metadata and basic image characteristics. A photograph can have several descriptive tags but one proposed destination.

Rules and manual corrections take precedence over broad visual guesses.

GO does not move files. It shows the proposed result. Export and direct file operations are separate actions that require confirmation.

Exact duplicate results compare file contents. Visually similar matches are suggestions for inspection. A resized or recompressed photograph may look identical but contain different data.

### Browsers and file access

The HTML runs without a server, but browser permissions determine which operations are available.

Choose files and ZIP export provide an alternative when direct folder writing is unavailable.

Direct Copy and Move require compatible browser filesystem support and permission from you. On some mobile browsers, you may need to extract the exported ZIP yourself to create the organised directories.

Large exports depend on available memory and filesystem support. Streaming ZIP output is used where supported; the fallback has more restrictive size limits.

### Privacy and safety

Files are analysed in your browser and are not uploaded by the application.

Metadata comments and embedded instructions are treated as file content, not commands. The application never automatically deletes suspected duplicates.

Copy is the sensible default. Move can remove an original after its destination has been written and verified, so keep an independent backup.

Recovery records and Undo help after an interruption but cannot guarantee recovery from every browser crash, storage failure or concurrent change outside the application.

Photograph classification is approximate. Review uncertain categories before committing an organisation run.

### Project format

The application is self-contained in one HTML file. It uses HTML, CSS and vanilla JavaScript, with no server, build process or external dependencies.

Current release: v1.1.2

### Licence

MIT Licence.

Copyright © 2025 TABARC-Code.

Created under TABARC-Studio.

TABARC-Code webpage repository

TABARC website


