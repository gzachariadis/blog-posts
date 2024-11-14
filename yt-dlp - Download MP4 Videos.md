
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