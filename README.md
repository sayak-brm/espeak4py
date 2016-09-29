## espeak TTS Bindings for Python3

###### Licenced under GNU GPLv3. Contains precompiled binaries for espeak v1.48.04. Sources for included binaries available [here](http://espeak.sourceforge.net/).
[![Build status](https://ci.appveyor.com/api/projects/status/o2j9pe6sttd0j684?svg=true)](https://ci.appveyor.com/project/sayak-brm/espeak4py) [![Build Status](https://travis-ci.org/sayak-brm/espeak4py.svg?branch=master)](https://travis-ci.org/sayak-brm/espeak4py) [![Code Climate](https://codeclimate.com/github/sayak-brm/espeak4py/badges/gpa.svg)](https://codeclimate.com/github/sayak-brm/espeak4py) [![Test Coverage](https://codeclimate.com/github/sayak-brm/espeak4py/badges/coverage.svg)](https://codeclimate.com/github/sayak-brm/espeak4py/coverage) [![Issue Count](https://codeclimate.com/github/sayak-brm/espeak4py/badges/issue_count.svg)](https://codeclimate.com/github/sayak-brm/espeak4py) [![Python Version](https://img.shields.io/badge/Python-3-brightgreen.svg)](https://www.python.org/download/releases/3.0/) [![espeak Version](https://img.shields.io/badge/espeak-v1.48.04-brightgreen.svg)](http://espeak.sourceforge.net/) ![Linux](https://img.shields.io/badge/Linux--brightred.svg) ![Windows](https://img.shields.io/badge/Windows--brightgreen.svg)

### Usage:

```python
import espeak4py

espeak4py.say('Hello, World!')
```

The above will stop interrupt any ongoing speech.
Code to wait for any ongoing speech to complete:

```python
espeak4py.say('I am a demo of the say() function.', wait4prev=True)
```

#### Changing speech properties:

###### Pitch:

By default the pitch is set at 80.

Change it by:

```python
espeak4py.say('I am a demo of the say function', pitch=120)
```

###### Words per Minute:

By default WPM is set at 120.

Change it by:

```python
espeak4py.say('I am a demo of the say function', wpm=140)
```

###### Voice:

By default WPM is set to 'en'.
Uses voice file of set name from `espeak-data/voices`.

Change it by:

```python
espeak4py.say('I am a demo of the say function', voice="es")
```