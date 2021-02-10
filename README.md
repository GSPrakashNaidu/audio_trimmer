# audiotrimmer

 A plugin to cut audio files. You pass in a path to a file, start and end times and the plugin will
 do the rest. For now, it automatically will reduce the quality quite a bit to ensure optimal file size for storage/streaming.

## Getting Started

0. Take a look at the requirements and any gotchas for your platform at the [flutter_ffmpeg](https://pub.dev/packages/flutter_ffmpeg)
package page. There can be some stumbling blocks getting it working on iOS. (Works on my machine ¯\\\_(ツ)_/¯)

1. Import and cut!

```
    import 'package:audio_trimmer/audio_trimmer.dart';

    {...}

    var start = 15.0;
    var end = 25.5;
    var path = 'path/to/audio/file.mp3';

    // Get path to cut file and do whatever you want with it.
    var outputFilePath = await AudioTrimmer.cutAudio(path, start, end);

```
