# discompress

A batch script to automatically compress video and audio files to under 25MB to allow for free upload to discord.

## Requirements

The script requires [FFmpeg](https://ffmpeg.org/download.html) to be installed on your system. Make sure FFmpeg is in your system's [path](https://phoenixnap.com/kb/ffmpeg-windows#ftoc-heading-4).

## Usage

To compress a video or audio file, simply drag and drop the file onto the batch script or use the terminal with the command `compress.bat <input_file>`.
The output file is saved as a .mp4 (if video) or a .mp3 (if audio) in the inputs file directory with the name 25MB_<input_filename>.

Path to batchfile can also be added to the registry to be able to compress in the windows right-click menu.

## Limitations

- Only supports video file extensions `.mp4 .avi .mkv .mov .flv .wmv .webm .mpeg .3gp`.
- Only supports audio file extensions `.mp3 .wav .m4a .flac .aac .ogg .wma`.
- Doesn't allow for compressions under 125kbps for video steam and 32kbps audio stream so longer files may not be able to be compressed.
- Requires FFmpeg to be installed on your systems path.

## Troubleshooting

If you encounter any issues while running the script, try the following:

1. Make sure FFmpeg is installed and in your system's path.
2. Make sure the input file has a valid extension (see "Limitations" section).
3. Make sure the input file is not already compressed to a size smaller than the target size or bitrate.
4. Make sure the output file does not already exist in the output directory.
5. If you still encounter issues, please contact the script author.

## License

This script is released under the [MIT License](https://opensource.org/licenses/MIT).
