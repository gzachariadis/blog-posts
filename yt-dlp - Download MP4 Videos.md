# yt-dlp

### General Options

- Continue with next video on download errors = --no-abort-on-error  ✔
- Do not load any more configuration files = --ignore-config  ✔
- DO not load any custom configuration files = --no-config-locations  ✔
- Mark Watched (default) = --no-mark-watched  ✔

### Network Options

- Client to impersonate for requests = --impersonate=chrome-99:windows-10
- Make all connections via IPV4 = --force-ipv4  ✔
- Geo-restriction = 

### Video Selection

- Download Archieve = --download-archive downloads.txt  ✔
- No Break on Existing = --no-break-on-existing  ✔

### Download Options

- Number of Retries = --retries infinite  ✔
- Number of tims to retry on file access = --file-access-retries infinite  ✔
- Number of retries for a fragment = --fragment-retries infinite  ✔
- Time to sleep between retries = --retry-sleep 5  ✔
- Delete downloaded fragments after downloading is finished = --no-keep-fragments  ✔
- Process videos in the playlist only after the entire playlist is parsed = --no-lazy-playlist  ✔

### Filesystem Options

- Video Title = -o "~/Downloads/Youtube/%(uploader)s - %(title)s"  ✔
- Force filenames to be Windows-compatible = --windows-filenames ✔
- Do not overwrite any files = --no-overwrites ✔
- Do not resume partially downloaded fragments = --no-continue ✔
- Do not use .part files - write directly into output files = --no-part ✔
- Do not use the last-modified header to set the file modification date = --no-mtime  ✔
- Do not write video description = --no-write-description  ✔
- Do not write video metadata = --no-write-info-json  ✔
- Do not write playlist metadata = --no-write-playlist-metafiles  ✔
- Remove some internal metadata such as filenames from the infojson = --clean-info-json  ✔
- Do not retrieve video comments = --no-get-comments --no-write-comments
- Do not read/dump cookies from/to file = --no-cookies  ✔
- Do not load cookies from browser = --no-cookies-from-browser  ✔
- Disable filesystem caching = --no-cache-dir  ✔
- Delete all filesystem cache files = --rm-cache-dir  ✔

### Thumbnail Options

- Do not write thumbnail image to disk = --no-write-thumbnail   ✔

### Internet Shortcut Options

### Verbosity and Simulation Options

- Show progress bar, even if in quiet mode = --progress   ✔
- Force download archive entries to be written as far as no errors occur = --force-write-archive  ✔

### Workarounds

- Number of secords to sleep between requests during data extraction = --sleep-requests 3   ✔
- Number of seconds to sleep before each download. = --sleep-interval 10   ✔

### Video Format Options

### Subtitle Options

- Do not write auto-generated subtitles = --no-write-auto-subs   ✔

### Authentication Options

### Post-Processsing Options

- Delete the intermediate video file on disk after post-processing = --no-keep-video
- Do not add metadata to file = --no-embed-metadata
- Do not embed the infojson as an attachment to the video file = --no-embed-info-json

### SponsorBlock Options

### Extractor Options

```--extractor-retries infinite```

```
yt-dlp \
--no-abort-on-error \
--ignore-config \
--no-config-locations \
--no-mark-watched \
--force-ipv4 \
--download-archive downloads.txt \
--no-break-on-existing \
--retries infinite \
--file-access-retries infinite \
--fragment-retries infinite \
--retry-sleep 5 \
--no-keep-fragments \
--no-lazy-playlist \
-o "~/Downloads/Youtube/%(uploader)s - %(title)s" \
--windows-filenames \
--no-overwrites \
--no-continue \
--no-part \
--no-mtime \
--no-write-description \
--no-write-info-json \
--no-write-playlist-metafiles \
--clean-info-json \
--no-write-comments \
--no-get-comments \
--no-cookies \
--no-cookies-from-browser \
--no-cache-dir \
--rm-cache-dir \
--no-write-thumbnail \
--progress \
--force-write-archive \
--sleep-requests 3 \
--sleep-interval 10 \
--no-write-auto-subs \
--no-keep-video \
--no-embed-metadata \
--no-embed-info-json \
-f bv+ba/b \
-S res,ext:mp4:m4a \
[link]
```