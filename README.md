# Vital

Vital is a spectral warping wavetable synthesizer.

## Code Licensing

If you are making a proprietary or closed source app and would like to use Vital's source code, contact licensing@vital.audio for non GPLv3 licensing options.

## Building

download (this vst sdk version)[https://web.archive.org/web/20181016150224/https://download.steinberg.net/sdk_downloads/vstsdk3610_11_06_2018_build_37.zip] (that is what the JUCE source files are calling for), extract it to `third_party/VST_SDK` and run the `copy_vst2_to_vst3_sdk.sh` script in that folder. build with make.

```shell
curl -LO https://web.archive.org/web/20181016150224/https://download.steinberg.net/sdk_downloads/vstsdk3610_11_06_2018_build_37.zip -o ./vstsdk3610_11_06_2018_build_37.zip
unzip -d third_party vstsdk3610_11_06_2018_build_37.zip
pushd third_part/VST_SDK
./copy_vst2_to_vst3_sdk.sh
popd
make -j32
sudo make install
```

## Installing

Create an account and download Vital at [vital.audio](https://vital.audio)

## Issues

Report issues to https://forum.vital.audio

I won't be checking issues on github on a regular basis.

## Pull requests

I will not take any pull requests.

## What can you do with the source

The source code is licensed under the GPLv3. If you download the source or create builds you must comply with that license.

### Things you can't do with this source

- Do not create an app and distribute it on the iOS app store. The app store is not comptabile with GPLv3 and you'll only get an exception for this if you're paying for a GPLv3 exception for Vital's source (see Code Licensing above).
- Do not use the name "Vital", "Vital Audio", "Tytel" or "Matt Tytel" for marketing or to name any distribution of binaries built with this source. This source code does not give you rights to infringe on trademarks.
- Do not connect to any web service at https://vital.audio, https://account.vital.audio or https://store.vital.audio from your own builds. This is against the terms of using those sites.
