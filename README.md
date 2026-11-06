# adrop-specs

CocoaPods spec repository for the [Adrop Ads SDK](https://adrop.io) — `adrop-ads` and `adrop-ads-backfill`.

New versions of these pods are published here. Earlier versions remain available from CocoaPods trunk.

## Usage

Add both sources at the top of your `Podfile`. Once a `source` line is present, CocoaPods no longer adds trunk implicitly, so the CDN line is required as well.

```ruby
source 'https://github.com/OpenRhapsody/adrop-specs.git'
source 'https://cdn.cocoapods.org/'
```

Then update the pods (include `adrop-ads-backfill` if you use it) and commit the updated `Podfile.lock`:

```sh
pod update adrop-ads adrop-ads-backfill
```

`pod install` alone keeps the versions and sources recorded in an existing `Podfile.lock`.
