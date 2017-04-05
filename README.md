# Python for Scientific Audio [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

The aim of this repository is to create a comprehensive, curated list of python software/tools related and used for scientific research in audio/music applications.

## Contents

* [Awesome Criteria](#awesome-criteria)
* [Related lists](#related-lists)
* [Audio Related Packages](#audio-related-packages)
    - [Read/Write](#read-write)
    - [Transformations - General DSP](#transformations---general-dsp)
    - [Feature extraction](#feature-extraction)
    - [Speech Processing](#speech-processing)
    - [Perceptial Models - Auditory Models](#perceptial-models---auditory-models)
    - [Source Separation](#source-separation)
    - [Music Information Retrieval](#music-information-retrieval)
    - [Symbolic Music - MIDI - Musicology](#symbolic-music---midi---musicology)
    - [Realtime applications](#realtime-applications)
    - [Web - Audio](#web---audio)
    - [Packages to access audio APIs - parsing audio datasets](#packages-to-access-audio-apis---parsing-audio-datasets)
    - [Wrappers for Audio Plugins](#wrappers-for-audio-plugins)
  + [Bindings or Wrappers for other languages](#bindings-or-wrappers-for-other-languages)
* [Tutorials - Books](#tutorials---books)
* [Contributing](#contributing)
  + [License](#license)
    
## Awesome Criteria

* the software is audio/music related
* the software is useful for several (not just one) fields of research
* (optional) the software is actively maintained (add a ⚠️ state if not)
* (optional) the software is listed on pypi (add a ⚠️ if not)
* (optional) the software runs on python 2 and python 3 (See `²` python 2 only, `³` for python 3 only)

## Related lists

There is already [PythonInMusic](https://wiki.python.org/moin/PythonInMusic) but it is not up to date and includes too many packages of special interest that are mostly not relevant for scientific applications. [Awesome-Python](https://github.com/vinta/awesome-python) is large curated list of python packages. However, the audio section is very small.

## Audio Related Packages

- Total number of packages: 58
- Python version compatibility:  ![12](http://progressed.io/bar/98?title=python%202) ![1](http://progressed.io/bar/79?title=python%203)

#### Read-Write

* [audiolazy](https://github.com/danilobellini/audiolazy) - Expressive Digital Signal Processing (DSP) package for Python
* [audioread](https://github.com/beetbox/audioread) - Cross-library (GStreamer + Core Audio + MAD + FFmpeg) audio decoding
* [pyAV](https://mikeboers.github.io/PyAV) - PyAV is a Pythonic binding for FFmpeg or Libav
* [(Py)Soundfile](https://github.com/bastibe/PySoundFile) - Library based on libsndfile, CFFI, and NumPy
* [pySox](https://github.com/rabitt/pysox) - Wrapper around sox
* [tinytag](https://github.com/devsnd/tinytag) - reading music meta data of MP3, OGG, FLAC and Wave files

#### Transformations - General DSP

* [AudioTK](https://github.com/mbrucher/AudioTK) - DSP filter toolbox (lots of filters)
* [Gammatone](https://github.com/detly/gammatone) - Gammatone filterbank implementation
* [pyFFTW3](https://github.com/pyFFTW/pyFFTW) - Wrapper around FFTW
* [NSGT](https://github.com/grrrr/nsgt)² - Non-stationary gabor transform, constant-q
* [MDCT](https://github.com/nils-werner/mdct) - MDCT transform
* [pydub](https://github.com/jiaaro/pydub) - Manipulate audio with a simple and easy high level interface
* [pytftb](https://github.com/scikit-signal/pytftb) - Implementation of the MATLAB Time-Frequency Toolbox
* [PyRubberband](https://github.com/bmcfee/pyrubberband) - Wrapper for [rubberband](http://breakfastquay.com/rubberband/) to do pitch-shifting and time-stretching
* [PyWavelets](https://github.com/scikit-signal/pywt)² - Discrete Wavelet Transform in Python
* [Resampy](https://github.com/bmcfee/resampy) - Sample rate conversion
* [STFT](https://github.com/nils-werner/stft) - Standalone package for Short-Time Fourier Transform 

#### Feature extraction

* [aubio](http://aubio.org/) - Feature extractor, written in C, python interface
* [audiolazy](https://github.com/danilobellini/audiolazy) - Realtime Audio Processing lib, general purpose
* [essentia](http://essentia.upf.edu) - C++ based feature extractor + general purpose audio/MIR related DSP algorithms like pitch tracking, beat detection
* [muda](https://github.com/bmcfee/muda) -  Musical Data Augmentation
* [python_speech_features](https://github.com/jameslyons/python_speech_features) - Common speech features for ASR
* [pyYAAFE](http://yaafe.sourceforge.net) - Python bindings for YAAFE

#### Speech Processing

* [pyAudioAnalysis](https://github.com/tyiannak/pyAudioAnalysis)² - Feature Extraction, Classification, Diarization
* [py-webrtcvad](https://github.com/wiseman/py-webrtcvad) -  Interface to the WebRTC Voice Activity Detector
* [SIDEKIT](http://lium.univ-lemans.fr/sidekit/)³ - Speaker and Language recognition
* [SpeechRecognition](https://github.com/Uberi/speech_recognition) -  Wrapper for several ASR engines and APIs, online and offline
* [talkbox](http://scikits.appspot.com/talkbox)² - General speech/signal processing algorithms. ⚠️ Not maintained

#### Perceptial Models - Auditory Models

* [cochlea](https://github.com/mrkrd/cochlea)² - Inner ear models
* [BrianHears](http://www.briansimulator.org/docs/index.html)² - General Auditory Models
* [Loudness](https://github.com/deeuu/loudness)² - Perceived loudness, includes Zwicker, Moore/Glasberg model
* [Sound Field Synthesis Toolbox](https://github.com/sfstoolbox/sfs-python) - Sound Field Synthesis Toolbox

#### Source Separation

* [beta_ntf](https://code.google.com/archive/p/beta-ntf/)² - Non-Negative Tensor factorisation using PARAFAC
* [commonfate](https://github.com/aliutkus/commonfate) - Common Fate Transform
* [NUSSL](https://github.com/interactiveaudiolab/nussl)² - Various source separation algorithms + framework
* [NTFLib](https://github.com/stitchfix/NTFLib) - Sparse Beta-Divergence Tensor Factorization Library
* [NIMFA](http://nimfa.biolab.si) - Several NMF flavors
* [pyFASST](https://github.com/wslihgt/pyfasst)² - Flexible Audio Source Separation Toolbox

#### Music Information Retrieval

* [Catchy](https://github.com/jvbalen/catchy) - Corpus Analysis Tools for Computational Hook Discovery
* [dejavu](https://github.com/worldveil/dejavu)² - Audio fingerprinting and recognition
* [Madmom](https://github.com/CPJKU/madmom) - MIR packages with strong focus on beat detection, onset detection and chord recognition
* [mir_eval](https://github.com/craffel/mir_eval) - Common scores for various MIR tasks. Also includes bss_eval implementation
* [librosa](https://github.com/librosa/librosa) - general audio and music analysis

#### Symbolic Music - MIDI - Musicology

* [Music21](http://web.mit.edu/music21/) - Toolkit for Computer-Aided Musicology
* [Mido](https://mido.readthedocs.io/en/latest/) - Realtime MIDI wrapper
* [mingus](http://bspaans.github.io/python-mingus/)² - Advanced music theory and notation package with MIDI file and playback support
* [Pretty-MIDI](https://github.com/craffel/pretty-midi) - Utility functions for handling MIDI data in a nice/intuitive way

#### Realtime applications

* [PYO](https://github.com/belangeo/pyo) - Realtime audio engine similar supercollider
* [python-sounddevice](https://github.com/spatialaudio/python-sounddevice) - another PortAudio wrapper
* [(Py)Soundcard](https://github.com/bastibe/PySoundCard) - PortAudio based realtime audio processing

#### Web + Audio

* [TimeSide](https://github.com/Parisson/TimeSide)² - Open web audio processing framework.

#### Packages to access audio APIs - parsing audio datasets

* [beets](http://beets.io/) - Music library manager and [MusicBrainz](https://musicbrainz.org/) tagger
* [dsdtools](https://github.com/faroit/dsdtools) - Parse and process the demixing secrets dataset
* [medleydb](https://github.com/marl/medleydb) - Parse medleydb audio + annotations
* [Soundcloud API](https://github.com/soundcloud/soundcloud-python) - Wrapper around the Soundcloud API
* [Youtube-Downloader](https://github.com/rg3/youtube-dl) - Download youtube videos (and the audio)

#### Wrappers for Audio Plugins

* [PyAU](https://github.com/simlmx/pyau)² ⚠️ Not maintained - Python Audio Unit Host
* [VamPy Host](https://code.soundsoftware.ac.uk/projects/vampy-host) - Interface compiled vamp plugins

### Bindings or Wrappers for other languages

* [CFFI]() - Easily interface c libraries
* [Matlab_Wrapper](https://github.com/mrkrd/matlab_wrapper) - Runs code in matlab and returns results to python
* [pybind11](https://pypi.python.org/pypi/pybind11) - Interface c++ code
* [rpy2](http://rpy2.bitbucket.org/) - Call R from python

## Tutorials - Books

* [Introduction to Numpy and Scipy](http://www.scipy-lectures.org/index.html) - Highly recommended :+1: 
* [Python Data Science Handbook](https://github.com/jakevdp/PythonDataScienceHandbook) - Excellent Book, look for the Tutorial notebooks
* [MIR Notebooks](http://musicinformationretrieval.com/)
* [From Python to Numpy](http://www.labri.fr/perso/nrougier/from-python-to-numpy/)
* https://github.com/spatialaudio/selected-topics-in-audio-signal-processing-exercises
* https://github.com/unpingco/Python-for-Signal-Processing

## Contributing

Your contributions are always welcome! Please take a look at the [contribution guidelines](CONTRIBUTING.md) first.

I will keep some pull requests open if I'm not sure whether those libraries are awesome, you could vote for them by adding 👍 to them.

### License

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](http://creativecommons.org/licenses/by/4.0/)
