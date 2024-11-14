# How to Remove Metadata From MP4 Files

```sh
exiftool -overwrite_original_in_place -all= /path/to/file
```

```sh
ffmpeg -i /path/to/input.mp4 -map 0 -map_metadata -1 -c copy /path/to/output.mp4
```

```sh
exiftool -r -overwrite_original_in_place -ext mp4 -all:all= ~/Downloads/Youtube

for file in ~/Downloads/Youtube/*; do
	ffmpeg -i ~/Downloads/Youtube/"${file##*/}" -map 0 -map_metadata -1 -c copy ~/Downloads/Metadata/"${file##*/}"
done
```

# References

- https://herrbischoff.com/2020/09/how-to-remove-metadata-from-mp4-files/

