# Python for Scientific Audio [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![Build Status](https://travis-ci.org/faroit/awesome-python-scientific-audio.svg?branch=master)](https://travis-ci.org/faroit/awesome-python-scientific-audio)

The aim of this repository is to create a comprehensive, curated list of python software/tools related and used for scientific research in audio/music applications.

## Contents

* [Audio Related Packages](#audio-related-packages)
    - [Read/Write](#read-write)
    - [Transformations - General DSP](#transformations---general-dsp)
    - [Feature extraction](#feature-extraction)
    - [Speech Processing](#speech-processing)
    - [Perceptial Models - Auditory Models](#perceptial-models---auditory-models)
    - [Source Separation](#source-separation)
    - [Music Information Retrieval](#music-information-retrieval)
    - [Deep Learning](#deep-learning)
    - [Symbolic Music - MIDI - Musicology](#symbolic-music---midi---musicology)
    - [Realtime applications](#realtime-applications)
    - [Web - Audio](#web-audio)
    - [Audio related APIs and Datasets](#audio-related-apis-and-datasets)
    - [Wrappers for Audio Plugins](#wrappers-for-audio-plugins)
* [Tutorials](#tutorials)
* [Books](#books)
* [Scientific Paper](#scientific-papers)
* [Other Resources](#other-resources)
* [Related lists](#related-lists)
* [Contributing](#contributing)
* [License](#license)


## Audio Related Packages

- Total number of packages: 72
- Python version compatibility:  ![69](http://progressed.io/bar/96?title=python%202) ![63](http://progressed.io/bar/86?title=python%203) (²indicates a python 2 only package, ³indicates a python 3 only package; the remaining package support python 2+3).

#### Read-Write

* [audiolazy](https://github.com/danilobellini/audiolazy) [:octocat:](https://github.com/danilobellini/audiolazy) [:package:](https://pypi.python.org/pypi/audiolazy/) - Expressive Digital Signal Processing (DSP) package for Python.
* [audioread](https://github.com/beetbox/audioread) [:octocat:](https://github.com/beetbox/audioread) [:package:](https://pypi.python.org/pypi/audioread/) - Cross-library (GStreamer + Core Audio + MAD + FFmpeg) audio decoding.
* [mutagen](https://mutagen.readthedocs.io/) [:octocat:](https://github.com/quodlibet/mutagen) [:package:](https://pypi.python.org/pypi/mutagen) - Reads and writes all kind of audio metadata for various formats.
* [pyAV](https://mikeboers.github.io/PyAV/) [:octocat:](https://mikeboers.github.io/PyAV/) - PyAV is a Pythonic binding for FFmpeg or Libav.
* [(Py)Soundfile](http://pysoundfile.readthedocs.io/) [:octocat:](https://github.com/bastibe/PySoundFile) [:package:](https://pypi.python.org/pypi/SoundFile) - Library based on libsndfile, CFFI, and NumPy.
* [pySox](https://github.com/rabitt/pysox) [:octocat:](https://github.com/rabitt/pysox) [:package:](https://pypi.python.org/pypi/pysox/) - Wrapper for sox.
* [PySynth](http://mdoege.github.io/PySynth) [:octocat:](https://github.com/mdoege/PySynth) - simple midi-to-wav synthesizer.
* [stempeg](https://github.com/faroit/stempeg) [:octocat:](https://github.com/faroit/stempeg) [:package:](https://pypi.python.org/pypi/stempeg/) - read/write of STEMS multistream audio.
* [tinytag](https://github.com/devsnd/tinytag) [:octocat:](https://github.com/devsnd/tinytag) [:package:](https://pypi.python.org/pypi/tinytag/) - reading music meta data of MP3, OGG, FLAC and Wave files.
* [audiomate](https://github.com/ynop/audiomate)³ [:octocat:](https://github.com/ynop/audiomate) [:package:](https://pypi.python.org/pypi/audiomate/) - Loading different types of audio datasets.

#### Transformations - General DSP

* [acoustics](http://python-acoustics.github.io/python-acoustics/) [:octocat:](https://github.com/python-acoustics/python-acoustics/) [:package:](https://pypi.python.org/pypi/acoustics) - useful tools for acousticians.
* [AudioTK](https://github.com/mbrucher/AudioTK) [:octocat:](https://github.com/mbrucher/AudioTK) - DSP filter toolbox (lots of filters).
* [AudioTSM](https://audiotsm.readthedocs.io/) [:octocat:](https://github.com/Muges/audiotsm) [:package:](https://pypi.python.org/pypi/audiotsm/) - real-time audio time-scale modification procedures.
* [Gammatone](https://github.com/detly/gammatone) [:octocat:](https://github.com/detly/gammatone) - Gammatone filterbank implementation.
* [pyFFTW](http://pyfftw.github.io/pyFFTW/) [:octocat:](https://github.com/pyFFTW/pyFFTW) [:package:](https://pypi.python.org/pypi/pyFFTW/) - Wrapper for FFTW(3).
* [NSGT](https://grrrr.org/research/software/nsgt/) [:octocat:](https://github.com/grrrr/nsgt) [:package:](https://pypi.python.org/pypi/nsgt) - Non-stationary gabor transform, constant-q.
* [MDCT](https://github.com/nils-werner/mdct) [:octocat:](https://github.com/nils-werner/mdct) [:package:](https://pypi.python.org/pypi/mdct) - MDCT transform.
* [pydub](http://pydub.com) [:octocat:](https://github.com/jiaaro/pydub) [:package:](https://pypi.python.org/pypi/mdct) - Manipulate audio with a simple and easy high level interface.
* [pytftb](http://tftb.nongnu.org) [:octocat:](https://github.com/scikit-signal/pytftb) - Implementation of the MATLAB Time-Frequency Toolbox.
* [pyroomacoustics](https://github.com/LCAV/pyroomacoustics) [:octocat:](https://github.com/LCAV/pyroomacoustics) [:package:](https://pypi.python.org/pypi/pyroomacoustics) - Room Acoustics Simulation (RIR generator)
* [PyRubberband](https://github.com/bmcfee/pyrubberband) [:octocat:](https://github.com/bmcfee/pyrubberband) [:package:](https://pypi.python.org/pypi/pyrubberband/) - Wrapper for [rubberband](http://breakfastquay.com/rubberband/) to do pitch-shifting and time-stretching.
* [PyWavelets](http://pywavelets.readthedocs.io) [:octocat:](https://github.com/PyWavelets/pywt) [:package:](https://pypi.python.org/pypi/PyWavelets) - Discrete Wavelet Transform in Python.
* [Resampy](http://resampy.readthedocs.io) [:octocat:](https://github.com/bmcfee/resampy) [:package:](https://pypi.python.org/pypi/resampy) - Sample rate conversion.
* [SFS-Python](http://sfstoolbox.org/) [:octocat:](https://github.com/sfstoolbox/sfs-python) [:package:](https://pypi.python.org/pypi/sfs/) - Sound Field Synthesis Toolbox.
* [STFT](http://stft.readthedocs.io) [:octocat:](https://github.com/nils-werner/stft) [:package:](https://pypi.python.org/pypi/stft) - Standalone package for Short-Time Fourier Transform.

#### Feature extraction

* [aubio](http://aubio.org/) [:octocat:](https://github.com/aubio/aubio) [:package:](https://pypi.python.org/pypi/aubio) - Feature extractor, written in C, Python interface.
* [audiolazy](https://github.com/danilobellini/audiolazy) [:octocat:](https://github.com/danilobellini/audiolazy) [:package:](https://pypi.python.org/pypi/audiolazy/) - Realtime Audio Processing lib, general purpose.
* [essentia](http://essentia.upf.edu) [:octocat:](https://github.com/MTG/essentia) - Music related low level and high level feature extractor, C++ based, includes Python bindings.
* [muda](https://muda.readthedocs.io/en/latest/) [:octocat:](https://github.com/bmcfee/muda) [:package:](https://pypi.python.org/pypi/muda) -  Musical Data Augmentation.
* [python_speech_features](https://github.com/jameslyons/python_speech_features) [:octocat:](https://github.com/jameslyons/python_speech_features) [:package:](https://pypi.python.org/pypi/python_speech_features) - Common speech features for ASR.
* [pyYAAFE](https://github.com/Yaafe/Yaafe) [:octocat:](https://github.com/Yaafe/Yaafe) - Python bindings for YAAFE feature extractor.
* [speechpy](https://github.com/astorfi/speechpy) [:octocat:](https://github.com/astorfi/speechpy) [:package:](https://pypi.python.org/pypi/speechpy) - Library for Speech Processing and Recognition, mostly feature extraction for now.

#### Speech Processing

* [aeneas](https://www.readbeyond.it/aeneas/) [:octocat:](https://github.com/readbeyond/aeneas/) [:package:](https://pypi.python.org/pypi/aeneas/) - Forced aligner, based on MFCC+DTW, 35+ languages.
* [Parselmouth](https://github.com/YannickJadoul/Parselmouth) [:octocat:](https://github.com/YannickJadoul/Parselmouth) [:package:](https://pypi.org/project/praat-parselmouth/) - Python interface to the [Praat](http://www.praat.org) phonetics and speech analysis, synthesis, and manipulation software.
* [pyAudioAnalysis](https://github.com/tyiannak/pyAudioAnalysis)² [:octocat:](https://github.com/tyiannak/pyAudioAnalysis) [:package:](https://pypi.python.org/pypi/pyAudioAnalysis/) - Feature Extraction, Classification, Diarization.
* [py-webrtcvad](https://github.com/wiseman/py-webrtcvad) [:octocat:](https://github.com/wiseman/py-webrtcvad) [:package:](https://pypi.python.org/pypi/webrtcvad/) -  Interface to the WebRTC Voice Activity Detector.
* [PyWorldVocoder](https://github.com/JeremyCCHsu/Python-Wrapper-for-World-Vocoder) [:octocat:](https://github.com/JeremyCCHsu/Python-Wrapper-for-World-Vocoder) - Wrapper for Morise's World Vocoder.
* [Montreal Forced Aligner](https://montrealcorpustools.github.io/Montreal-Forced-Aligner/) [:octocat:](https://github.com/MontrealCorpusTools/Montreal-Forced-Aligner) - Forced aligner, based on Kaldi (HMM), English (others can be trained).
* [SIDEKIT](http://lium.univ-lemans.fr/sidekit/)³ [:package:](https://pypi.python.org/pypi/SIDEKIT/) - Speaker and Language recognition.
* [SpeechRecognition](https://github.com/Uberi/speech_recognition) [:octocat:](https://github.com/Uberi/speech_recognition) [:package:](https://pypi.python.org/pypi/SpeechRecognition/) -  Wrapper for several ASR engines and APIs, online and offline.

#### Perceptial Models - Auditory Models

* [cochlea](https://github.com/mrkrd/cochlea)² [:octocat:](https://github.com/mrkrd/cochlea) [:package:](https://pypi.python.org/pypi/cochlea/) - Inner ear models.
* [Brian2](http://briansimulator.org/) [:octocat:](https://github.com/brian-team/brian2) [:package:](https://pypi.python.org/pypi/Brian2) - Spiking neural networks simulator, includes cochlea model.
* [Loudness](https://github.com/deeuu/loudness)³ [:octocat:](https://github.com/deeuu/loudness) - Perceived loudness, includes Zwicker, Moore/Glasberg model.
* [Sound Field Synthesis Toolbox](http://sfstoolbox.org/) [:octocat:](https://github.com/sfstoolbox/sfs-python) [:package:](https://pypi.python.org/pypi/sfs/) - Sound Field Synthesis Toolbox.

#### Source Separation

* [beta_ntf](https://code.google.com/archive/p/beta-ntf/)² [:octocat:](https://github.com/nils-werner/beta_ntf) - Non-Negative Tensor factorisation using PARAFAC.
* [commonfate](https://github.com/aliutkus/commonfate) [:octocat:]() [:package:](https://pypi.python.org/pypi/commonfate) - Common Fate Model and Transform.
* [NUSSL](https://interactiveaudiolab.github.io/nussl/)² [:octocat:](https://github.com/interactiveaudiolab/nussl) [:package:](https://pypi.python.org/pypi/nussl) - Various source separation algorithms + framework.
* [NTFLib](https://github.com/stitchfix/NTFLib) [:octocat:](https://github.com/stitchfix/NTFLib) - Sparse Beta-Divergence Tensor Factorization.
* [NIMFA](http://nimfa.biolab.si) [:octocat:](https://github.com/marinkaz/nimfa) [:package:](https://pypi.python.org/pypi/nimfa) - Several NMF flavors.
* [pyFASST](https://github.com/wslihgt/pyfasst)² [:octocat:](https://github.com/wslihgt/pyfasst) [:package:](https://pypi.python.org/pypi/pyFASST) - Wrapper for Flexible Audio Source Separation Toolbox.

#### Music Information Retrieval

* [Catchy](https://github.com/jvbalen/catchy) [:octocat:](https://github.com/jvbalen/catchy) - Corpus Analysis Tools for Computational Hook Discovery.
* [dejavu](http://willdrevo.com/fingerprinting-and-audio-recognition-with-python/)² [:octocat:](https://github.com/worldveil/dejavu) [:package:](https://pypi.python.org/pypi/PyDejavu) - Audio fingerprinting and recognition.
* [Madmom](https://madmom.readthedocs.io/en/latest/) [:octocat:](https://github.com/CPJKU/madmom) [:package:](https://pypi.python.org/pypi/madmom) - MIR packages with strong focus on beat detection, onset detection and chord recognition.
* [mir_eval](http://craffel.github.io/mir_eval/) [:octocat:](https://github.com/craffel/mir_eval) [:package:](https://pypi.python.org/pypi/mir_eval) - Common scores for various MIR tasks. Also includes bss_eval implementation.
* [msaf](http://pythonhosted.org/msaf/) [:octocat:](https://github.com/urinieto/msaf) [:package:](https://pypi.python.org/pypi/msaf) - Music Structure Analysis Framework.
* [librosa](http://librosa.github.io/librosa/) [:octocat:](https://github.com/librosa/librosa) [:package:](https://pypi.python.org/pypi/librosa) - General audio and music analysis.
* [rp_extract](https://github.com/tuwien-musicir/rp_extract)² [:octocat:](https://github.com/tuwien-musicir/rp_extract) - Rhythm Pattern music feature extractor.

#### Deep Learning

* [Kapre](https://github.com/keunwoochoi/kapre) [:octocat:](https://github.com/keunwoochoi/kapre) [:package:](https://pypi.python.org/pypi/kapre) - Keras Audio Preprocessors
* [TorchAudio](https://github.com/pytorch/audio) [:octocat:](https://github.com/pytorch/audio) - PyTorch Audio Loaders

#### Symbolic Music - MIDI - Musicology

* [Music21](http://web.mit.edu/music21/) [:octocat:](https://github.com/cuthbertLab/music21) [:package:](https://pypi.python.org/pypi/music21) - Toolkit for Computer-Aided Musicology.
* [Mido](https://mido.readthedocs.io/en/latest/) [:octocat:](https://github.com/olemb/mido) [:package:](https://pypi.python.org/pypi/mido) - Realtime MIDI wrapper.
* [mingus](http://bspaans.github.io/python-mingus/)² [:octocat:](https://github.com/bspaans/python-mingus) [:package:](https://pypi.python.org/pypi/mingus/) - Advanced music theory and notation package with MIDI file and playback support.
* [Pretty-MIDI](http://craffel.github.io/pretty-midi/) [:octocat:](https://github.com/craffel/pretty-midi) [:package:](https://pypi.python.org/pypi/pretty-midi) - Utility functions for handling MIDI data in a nice/intuitive way.

#### Realtime applications

* [PYO](http://ajaxsoundstudio.com/software/pyo/) [:octocat:](https://github.com/belangeo/pyo) - Realtime audio dsp engine.
* [python-sounddevice](https://github.com/spatialaudio/python-sounddevice) [:octocat:](http://python-sounddevice.readthedocs.io) [:package:](https://pypi.python.org/pypi/sounddevice) - PortAudio wrapper providing realtime audio I/O with NumPy.

#### Web Audio

* [TimeSide](https://github.com/Parisson/TimeSide)² [:octocat:](https://github.com/Parisson/TimeSide) - high level audio analysis, imaging, transcoding, streaming and labelling.

#### Audio related APIs and Datasets

* [beets](http://beets.io/) [:octocat:](https://github.com/beetbox/beets) [:package:](https://pypi.python.org/pypi/beets) - Music library manager and [MusicBrainz](https://musicbrainz.org/) tagger.
* [dsdtools](http://dsdtools.readthedocs.io) [:octocat:](https://github.com/faroit/dsdtools) [:package:](https://pypi.python.org/pypi/dsdtools) - Parse and process the [demixing secrets dataset](http://sisec17.audiolabs-erlangen.de/#/dataset).
* [medleydb](http://medleydb.readthedocs.io) [:octocat:](https://github.com/marl/medleydb) - Parse [medleydb](http://medleydb.weebly.com/) audio + annotations.
* [Soundcloud API](https://github.com/soundcloud/soundcloud-python) [:octocat:](https://github.com/soundcloud/soundcloud-python) [:package:](https://pypi.python.org/pypi/soundcloud) - Wrapper for [Soundcloud API](https://developers.soundcloud.com/).
* [Youtube-Downloader](http://rg3.github.io/youtube-dl/) [:octocat:](https://github.com/rg3/youtube-dl) [:package:](https://pypi.python.org/pypi/youtube_dl) - Download youtube videos (and the audio).

#### Wrappers for Audio Plugins

* [VamPy Host](https://code.soundsoftware.ac.uk/projects/vampy-host) [:package:](https://pypi.python.org/pypi/vamp) - Interface compiled vamp plugins.

## Tutorials

* [Whirlwind Tour Of Python](https://jakevdp.github.io/WhirlwindTourOfPython/) [:octocat:](https://github.com/jakevdp/WhirlwindTourOfPython
) - fast-paced introduction to Python essentials, aimed at researchers and developers.
* [Introduction to Numpy and Scipy](http://www.scipy-lectures.org/index.html) [:octocat:](https://github.com/scipy-lectures/scipy-lecture-notes) - Highly recommended tutorial, covers large parts of the scientific Python ecosystem.
* [Numpy for MATLAB® Users](https://docs.scipy.org/doc/numpy/user/numpy-for-matlab-users.html) - Short overview of equivalent python functions for switchers.
* [MIR Notebooks](http://musicinformationretrieval.com/) [:octocat:](https://github.com/stevetjoa/stanford-mir) - collection of instructional iPython Notebooks for music information retrieval (MIR).
* [Selected Topics in Audio Signal Processing]( https://github.com/spatialaudio/selected-topics-in-audio-signal-processing-exercises) - Exercises as iPython notebooks.

## Books

* [Python Data Science Handbook](https://github.com/jakevdp/PythonDataScienceHandbook) - Jake Vanderplas, Excellent Book and accompanying tutorial notebooks.
* [Fundamentals of Music Processing](https://www.audiolabs-erlangen.de/fau/professor/mueller/bookFMP) - Meinard Müller, comes with Python exercises.

## Scientific Papers

* [Python for audio signal processing](http://eprints.maynoothuniversity.ie/4115/1/40.pdf) - John C. Glover, Victor Lazzarini and Joseph Timoney, Linux Audio Conference 2011.
* [librosa: Audio and Music Signal Analysis in Python](http://conference.scipy.org/proceedings/scipy2015/pdfs/brian_mcfee.pdf), [Video](https://www.youtube.com/watch?v=MhOdbtPhbLU) - Brian McFee, Colin Raffel, Dawen Liang, Daniel P.W. Ellis, Matt McVicar, Eric Battenberg, Oriol Nieto, Scipy 2015.

## Other Resources

* [Coursera Course](https://www.coursera.org/learn/audio-signal-processing) -  Audio Signal Processing, Python based course from UPF of Barcelona and Stanford University.
* [Digital Signal Processing Course](http://dsp-nbsphinx.readthedocs.io/en/nbsphinx-experiment/index.html) - Masters Course Material (University of Rostock) with many Python examples.
* [Slack Channel](https://mircommunity.slack.com) - Music Information Retrieval Community.

## Related lists

There is already [PythonInMusic](https://wiki.python.org/moin/PythonInMusic) but it is not up to date and includes too many packages of special interest that are mostly not relevant for scientific applications. [Awesome-Python](https://github.com/vinta/awesome-python) is large curated list of python packages. However, the audio section is very small.

## Contributing

Your contributions are always welcome! Please take a look at the [contribution guidelines](CONTRIBUTING.md) first.

I will keep some pull requests open if I'm not sure whether those libraries are awesome, you could vote for them by adding 👍 to them.

## License

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
