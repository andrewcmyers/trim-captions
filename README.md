# trim-captions
A script to convert Zoom captions into Kaltura captions while supporting video editing.

This lets you record on Zoom and edit video in Kaltura while keeping the higher-quality Zoom captions. If you delete video segments in Kaltura then you tell the script the timestamps (with the `-d` option); it removes captions and adjusts caption timestamps accordingly.

## Example

```
trim-captions -d 0-38.4 -d 2:34-2:51.40 Zoom.vtt > Zoom.srt
```

This command converts `Zoom.vtt` to produce `Zoom.srt`, deleting the first 38.4 seconds and also a 7.4 second segment starting at 2:34.
