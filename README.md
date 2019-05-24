# Home WatchDog

This is a quick dirty home surveillance setup using a Raspi. It uses a Raspberry Pi 3 with a PiCam and detects any kind of movement in the room. If there is a movement, it captures the frame and uploads it to Dropbox (if configured).

This is the initial work by Adrian and I will be extending on this by including a motion sensor and some Telegram API alerts along with IFTTT implementation.

Yay Home Project!!!

### Install Dependencies

- Install Dropbox
```sh
$ pip install dropbox
```

Install Imaging Processing utilities
```sh
$ pip install imutils
```

Install PiCam libs
```
$ pip install "picamera"
```

### Configuration

Options are configurable in the `config.json` that need to be passed at runtime.

### Execution

Start the watchdog with the following command

```sh
$ python pi_surveillance.py --conf conf.json
```



Credits: Adrian Rosebrock
