# AI-CHESS
AI-Chess is a AI based voice recognition chess game. The user may play against a friend or the computer(AI) by using mouse or voice commands.

## Installation
### Speech Recognition

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Speech Recognition

```bash
pip install SpeechRecognition
```
### PyAudio

 Go to this link -> [PyAudio](https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyaudio)

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install PyAudio

```bash
pip install PyAudio‑0.2.11‑cp39‑cp39‑win_amd64.whl
```
## Description
The AI that plays against the human evaluates all possible moves made by either
player up to a certain level of depth. The AI evaluates each position by giving
it a score. The higher the value of the score, the more favourable a position
is for white and the lower the value of the score, the more favourable the
position is for black. Knowing that white will try to get the score to be higher
and black will try and get the score to be lower, the AI assumes best play from
either side as it traverses up the search tree and chooses the best move to be
played.
## Usage

### Initializing Speech Recognition
 
```python
 import speech_recognition as sr

 self.r = sr.Recognizer()
 self.r.dynamic_energy_threshold = False
 self.r.energy_threshold = 400
```
### Speech Recognizing Using Google

```python
import speech_recognition as sr

with sr.Microphone() as source:
    self.r.adjust_for_ambient_noise(source)
    pygame.mixer.Sound.play(self.selectpiece_sound)
    time.sleep(1.5)
    try:
        audio = self.r.listen(source,timeout=2,phrase_time_limit=2)
        print("Recognizing...")
        query = self.r.recognize_google(audio)
        print(f"User said: {query}\n")
        voice = query.lower()
```


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Support
[Gmail](modimanju2019@gmail.com)

