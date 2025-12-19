---
authors:
  - name: null
---

# 2 Creating Digital Audio

## 2.1 General Considerations

The process and considerations involved in creating digital audio files are fully discussed in a number of JISC Digital Media documents, specifically:

* 'Choosing a Digital Audio File Format'
* 'Basic Audio Editing'
* 'Choosing a Digital Audio File Format'

As discussed in Section 1, the quality of the file is the key consideration when creating digital audio files. In order to ensure that the file being created is of a suitable quality and fit for purpose, data creators should be aware of :

* the relationship between audio container or 'wrapper' formats and the codecs that they contain as well as their respective capabilities.
* the fact that, as a component of the codec, audio formats can feature both lossless and lossy compression or come in uncompressed formats. Data creators should be aware of how these affect both data quality and file size at at what stages in the work flow these options will (if at all) be used.
* that many files allow metadata to be embedded within the container format and that data creators may want to utilise this functionality to record important aspects of the data creation process. Steps should be taken to identify or flag up this metadata where it exists so that it can be maintained regardless of format.
* which rights exist (e.g. copyright or moral right). This is particularly relevant to interview situations and data creators should be aware of any ethical implications of their work. In all cases clearance/permission should be sought from those involved in the recording. These issues are discussed in the JISC Digital Media document 'Copyright and Other Rights for Creating Time-based Media Resources'.

As a general guide - and one that is repeated throughout these Guides - it is advised that data creators create (and archive) audio data at as high a quality level as is available and in an uncompressed format. From this master dataset, lower filesize/quality datasets can be derived via format migratation or downsampling.

## 2.2 File Formats

```{list-table}
:header-rows: 1

* - Format
  - Properties/Technologies
  - Description
  - Recommendations
* - Waveform Audio (.wav)
  - A widely used and openly documented (though proprietary) container format developed by Microsoft and IBM.
  - The .wav format is commonly used to store uncompressed audio (as PCM) but can also contain audio in a variety of lossy codecs such as MP3. The format can also be tagged with metadata and can embed metadata in the XMP format.
  - Suitable for preservation depending on the codec used.
* - Audio Interchange File Format (.aif, .aiff)
  - Proprietary format developed by Apple and similar to the .wav format.
  - As with .wav, the .aiff is predominantly used for storing uncompressed PCM audio files. The format is also capable of storing metadata along with audio in other compressed codec formats.
  - Suitable for preservation in uncompressed format.
* - Sun AU (.au)
  - A format developed by Sun for Unix systems.
  - As with .wav and .aif files, Sun AU files tend to be large and of high quality but are not widely supported outside the UNIX community. Although predominantly using PCM encoding, .au files can support a number of of other codecs.
  - Not widely supported outside the UNIX community so therefore not suitable for preservation. 
* - Advanced Audio Coding (.aac)
  - An ISO standard format based on MPEG-2 and MPEG-4 formats
  - The format is widely supported by a number of common devices (Wii, Playstation, iPod, iPhone amongst others) and is designed to be the successor of the MP3 format. AAC format data may be commonly packaged in MP4, 3GP, ADIF and ADTS container formats.
  - Suiatble for dissemination but not for preservation.  
* - Broadcast Wave Format (BWF) (.bwf .wav)
  - A [specification of the European Broadcasting Union](https://tech.ebu.ch/docs/tech/tech3285.pdf) and an extension of the WAV format.
  - Broadcast Wave Format consists of uncompressed audio that extends the WAV format with an additional 'chunk' for metadata. Although based on the same format, compatibility between WAV and BWF files can be problematic, particularly when migrating WAV to BWF.
  - Suitable for preservation.
* - Ogg Vorbis (.ogg)
  - A non-proprietary open format developed by Xiph.org.
  - The Vorbis codec has been developed as a completely open alternative to the MP3 format and primarily as a dissemination format (the Ogg wrapper format can also contain codecs other than Vorbis e.g. FLAC).
  - Suitable as a dissemination format.
* - MP3 (.mp3)
  - A popular ISO standard format and part of the MPEG-1 and 2 standards
  - .MP3 (or MPEG-1 Audio Layer 3) is a lossy format that also allows metadata (ID3) to be embedded within a file.
  - Suitable for dissemination but not for preservation.
* - MPEG-4 (.m4a, .m4p)
  - An ISO standard container format
  - The MPEG-4 format supports a number of different audio codecs (e.g. AAC, MP3) as well as embedded metadata (including XMP). The format is commonly used by Apple's iTunes store although files sold here commonly feature encrypted audio stream and can be identified by the .m4p suffix.
  - Suitable for dissemination.
* - RealAudio (.ra, .ram)
  - A proprietary audio codec developed by RealNetworks.
  - RealAudio files can use a number of codecs including the RealAudio Lossless Format (ralf). Developed partly for streaming media, users should be aware that some files (e.g. .ram) are merely links to online files rather than files in themselves.
  - Not suitable for preservation.
* - Windows Media Audio (.wma, .asf)
  - A proprietary format developed by Microsoft encompassing a number of codecs and a container format.
  - The WMA set of codecs includes lossless, voice-specific and 'professional' variants of the standard format. In addition, WMA data is often wrapped with the proprietary ASF container.
  - Not suitable for preservation.
* - FLAC (.flac)
  - FLAC (Free Lossless Audio Codec) is an open and free lossless compression codec developed by Xiph.Org Foundation
  - FLAC has been developed as an open-source, lossless and more efficient alternative to the MP3 format and has been growing in popularity. FLAC encoded audio can be embedded in various different container formats including 'Native Flac' and Ogg.
  - Suitable for dissemination and may have use as a preservation format where compression is required.
* - Speex (.ogg)
  - An open, free codec developed by the [Xiph.Org](http://www.xiph.org) Foundation
  - As with other Xiph.Org Foundation formats (e.g. Vorbis, FLAC), Speex is a free and open codec. Speex is targetted specifically at providing high quality compressed voice/speech files.
  - Suitable for dissemination but not for preservation.
```