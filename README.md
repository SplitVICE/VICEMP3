# A simple Audio JavaScript class
### Usage
```
let audio = undefined, mp3_path = './wave.mp3'
const set = () => { audio = new VICEMP3(mp3_path, 1, true) }
set()

audio.play() // plays audio

audio.stop() // stops audio

audio.toggle // plays if stopped, stops if playing

// Restarts audio to the beginning
function restart() {
    audio.stop() // comment this line to make multiple audios play
    set()
}

// Sets a new volume level. Min = 0.1 ; Max = 1
function volume_set(volume) { audio.setVolume(volume) }
```