# ffmpeg_video_recorder

This is a python desktop video recorder using ffmepg.

## Getting Started

### Prerequisites

- ffmpeg

    Mac OS
    
    ```
    $ brew install ffmpeg
    ```

### Running

You can run it directly by

```
$ python3 video_recorder.py
```

And you will see

<img src="https://raw.githubusercontent.com/josephzxy/pic/master/Screen%20Shot%202018-07-20%20at%204.12.42%20PM.png" height=140>

Click `save as` to specify the path to save the video before recording.

Then click `record` to start recording.

To stop recording, simply click `stop` and the file will be saved.

<img src="https://raw.githubusercontent.com/josephzxy/pic/master/Screen%20Shot%202018-07-20%20at%204.13.23%20PM.png" height=140>

#### Note
- The name of the video will be set as the unix timestamp of when you click `record` by default.

### Possible Trouble shooting

#### 0: Input/output error

```
[avfoundation @ 0x7fd31e002600] Supported modes:
[avfoundation @ 0x7fd31e002600]   1280x720@[1.000000 30.000000]fps
    Last message repeated 2 times
0: Input/output error
```
Change the value of `-framerate` to an appropriate value according to  the supported modes information in the error message.

E.g. in the case above, change the value of `-framerate` to a value in  `1.000000 30.000000]`


## Built With

* [ffmpeg](https://www.ffmpeg.org/) - The video recording tool used


## Authors

* **Joseph Chu** - *Initial work* - [josephzxy](https://github.com/josephzxy)


## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details


