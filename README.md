# MP3 Cutter

MP3 Cutter is a JavaScript library and a NodeJS module that allows you to cut your MP3 files by seconds.

## Usage

```
const MP3Cutter = require('mp3-cutter');

const sendData = async (req, res) => {
    MP3Cutter.cut({
    src: 'source.mp3',
    responseObj: res,
    start: 25,
    end: 70
});
}


```

### Method

##### `cut(Object options)`

#### Options

##### `src {String}`

Path to the file to be cut.

##### `responseObj {Object}`

HTTP response object

##### `start {Number}`

Start position in seconds.

##### `end {Number}`

End position in seconds.

### CLI Tool

You can also use MP3 Cutter on the command line.

```
$ npm install -g mp3-cutter
$ mp3-cutter --src source.mp3 --target target.mp3 --start 10 --end 50
```

## License

MP3 Cutter is provided under the [MIT License](https://opensource.org/licenses/MIT).
