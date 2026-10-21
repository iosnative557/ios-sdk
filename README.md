# ios-sdk

The iOS SDK and the Swift / clang toolchain libraries, extracted from Xcode with
[ios-sdk-extractor](https://github.com/iosnative557/ios-sdk-extractor), ready to use with a
separately installed Swift toolchain.

## Contents

| Directory | Xcode | iOS SDK | Swift |
|---|---|---|---|
| [`27/`](27) | 27.1 | 27.1 | 6.4.0 |


## Use

1. Unzip `iPhoneOS.platform.zip` into a directory of your choice, e.g. `sdk/`, which gives
   `sdk/iPhoneOS.platform/Developer/SDKs/iPhoneOS.sdk`.
2. Unzip `toolchain.zip` into its own directory, e.g. `toolchain/`, which gives
   `toolchain/usr/lib/swift/...` and `toolchain/usr/lib/clang/...`.

Use `unzip` on macOS or Linux: the zips store symbolic links as standard zip symlink entries,
and `unzip` restores them.


## Make your own

To extract a different Xcode version or other platforms (watchOS, tvOS, visionOS, macOS), use
[ios-sdk-extractor](https://github.com/iosnative557/ios-sdk-extractor) with an `Xcode_*.xip`
downloaded from [developer.apple.com](https://developer.apple.com/download/all/):

```sh
ios-sdk-extractor -x Xcode_27.xip -c iphone -o sdkextracted
```

## License

The files in this repository are Apple software, provided by Apple under the
[Xcode and Apple SDKs Agreement](https://www.apple.com/legal/sla/docs/xcode.pdf). Use them
in accordance with that agreement.
