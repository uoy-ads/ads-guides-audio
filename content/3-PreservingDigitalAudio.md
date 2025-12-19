---
authors:
  - name: 
---

# 3 Preserving Digital Audio

## 3.1 Deciding What to Archive

As stated throughout this guide and by @knight2005audio, "the moment of creation is the most important stage of digital audio preservation" and, where possible the original file should be preserved in a format which captures and maintains its significant properties (discussed below) at an equal or higher value. In addition to the physical characteristics of the file, any associated metadata and documentation (either embedded or stored separately) should also be preserved and maintained.

## 3.2 Deciding How to Archive

__Significant Properties__

The significant properties of audio files that should be maintained throughout preservation activities are discussed in detail in 'Significant Properties Testing Report: Audio Recordings.' [@knight2010inspect, 8-10]. These are summarised below:

* Duration - i.e. the length of the audio file in Timecode character format (TCF). Checks should be made to ensure that the file matches its intended length.
* Bit Depth - indicates the number of bits of information stored per sample and is an indicator of audio quality e.g. 16 or 24 bit.
* Sample Rate - an indicator of the number of samples per second, sample rate is usually expressed in hertz e.g. 44.1 kHz (a common sample rate) and is, like bit depth, an indicator of the quality of the file.
* Channels -  A descriptive or numeric value that indicates the number of distinct streams within an audio object or a description of their configuration e.g. "2 (stereo)".
* Channel Assignment: Channel Number and Sound Map Location - Two values that allow specific channels to be mapped to specific output locations to configure the output sound.

__File Formats__

The file formats outlined below are those recommended for the preservation of audio files. As highlight by the JISC Digital Media document 'Uncompressed Audio File Formats
', uncompressed audio formats provide "the most accurate digital representation of a soundwave, but can also be the most resource-intensive method of recording and storing digital audio". In light of this, uncompressed formats/codecs are highly recommended for the preservation of audio files but, where this is not possible, high quality lossless compression may be used (e.g. FLAC).

```{list-table}
:header-rows: 1

* - Preservation Format
  - Requirements
* - Waveform Audio (.wav)
  - Recommended for preservation using uncompressed audio (PCM). The format can also be tagged with metadata and can embed metadata in the XMP format.
* - Broadcast Wave Format (BWF) (.bwf .wav)
  - Recommended for preservation, BWF also extends the WAV format with an additional 'chunk' for metadata although users should be aware that compatibility between WAV and BWF files can be problematic, particularly when migrating WAV to BWF.
* - Audio Interchange File Format (.aif, .aiff)
  - Suitable for preservation when used for storing uncompressed PCM audio files. The format is also capable of storing embedded metadata.
* - FLAC (.flac)
  - An open and free lossless compression codec, suitable for preservation when uncompressed audio is not desirable.
```

## 3.3 Metadata and Documentation

A number of different metadata schemes exist for audio files and the data type is notable in that many formats allow metadata to be embedded within the file itself. The metadata elements descibed below cover primaril technical aspects and form a minimum of what should be recorded. Generic [Project Metadata](https://doi.org/10.5284/h0p2-5584) should also be recorded.

```{list-table}
:header-rows: 1

* - Element
  - Description
* - Software
  - The software (or device) used to create the file.
* - Bit Depth
  - E.g. 16 or 24 bit.
* - Bit Rate
  - Optional, often recorded as kbps
* - Sample Rate (KHz)
  - E.g. 44.1kHz
* - Codec Used
  - The codec used in creating the file e.g. FLAC or AAC.
* - Length of Recording
  - Preferably recorded in hours, minutes, seconds (hh:mm:ss). 
* - Copyright Clearances
  - These are very important for audio files, especially oral histories/interviews.
* - Transcriptions of interviews
  - Transcripts of interviews can be important documentation particularly in clarifying those involved in recordings and allowing specific individuals to be identified.
```

Other metadata schemes are outlined by [IASA](https://www.iasa-web.org/tc04/basic-metadata) and discussed in detail by JISC Digital Media.

## 3.4 Copyright

As highlighted in Section 2, data creators should be aware of the various rights involved in recording people and should ensure that the relevant rights and clearances are attained. These issues are discussed in detail in the JISC Digital Media document 'Copyright and Other Rights for Creating Time-based Media Resources'.

----
