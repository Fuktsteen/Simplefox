# Simplefox
A simple list of [about:config](https://support.mozilla.org/en-US/kb/about-config-editor-firefox) tweaks to enhance [Mozilla Firefox](https://www.mozilla.org/en-US/firefox/new/).

Improves privacy and quality of life while maintaining a heavy emphasis on usability, ie.:

- disables telemetry, AI and speculative loading
- enables Strict Tracking Protection and DNS over HTTPS
- opts out of experiments and crash reports

## Instructions
0) Create a backup profile. Not needed, but recommended.
1) Download the `user.js` or `casual.js` file. (Rename `casual.js` to `user.js` after downloading!)
2) In Firefox, type `about:profiles` in the URL bar and press **Enter**.
3) For the profile you want to use, click **Open Folder** in the **Root Directory** section.
4) Move the `user.js` file into the folder.
5) Restart Firefox.
6) Optionally for added privacy install the [uBlock Origin](https://addons.mozilla.org/blog/ublock-origin-everything-you-need-to-know-about-the-ad-blocker/) content blocker.

[Betterfox](https://github.com/yokoffing/Betterfox) has great lists of common changes to the `user.js` (and `casual.js`) file: [Common Overrides](https://github.com/yokoffing/Betterfox/wiki/Common-Overrides) and [Optional Hardening](https://github.com/yokoffing/Betterfox/wiki/Optional-Hardening). Use to your preference.

## Which one is for me, `user.js` or `casual.js`?
While very similar, `casual.js` has some minor changes compared to `user.js` to ensure reliability.

1) Enables "Fix major site issues" under Enhanced Tracking Protection.
2) Removes alternative geo service.
3) Switches from "Max Protection" to "Increased Protection" under DNS over HTTPS.

`user.js` is very stable (personally never had any problems), but `casual.js` further ensures it.

## Heavily opinionated settings

1) Geo service provider - [BeaconDB](https://beacondb.net/)
2) DNS over HTTPS provider - [Mullvad](https://mullvad.net/en) (anti ad, tracker and malware [preset](https://mullvad.net/en/help/dns-over-https-and-dns-over-tls))

Should you prefer some other service providers, the respective settings have been located at the top of both `user.js` and `casual.js` files.

## What is `user.js`?
`user.js` is a configuration file you can use to change Firefox' [about:config](https://support.mozilla.org/en-US/kb/about-config-editor-firefox) settings in bulk.

Simplefox' `user.js` is a curated list of simple changes to improve the already great Firefox experience.

## How is Simplefox different from Betterfox or Arkenfox?
[Betterfox](https://github.com/yokoffing/Betterfox) and its parent project [Arkenfox](https://github.com/arkenfox/user.js) both use a `user.js` to improve the Firefox experience.

Simplefox is a shrunk fork of Betterfox to keep things simpler, mainly for my personal use.