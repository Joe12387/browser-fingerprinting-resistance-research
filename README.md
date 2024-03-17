# Browser Fingerprinting Resistance Research

This repo is a summary of current <a href="https://en.wikipedia.org/wiki/Device_fingerprint#Browser_fingerprint">browser fingerprinting</a> protections used by various browsers and their effectiveness against various fingerprinting techniques & services.

# Techniques

These are the known fingerprinting techniques & each browser's susceptibility to each for tracking purposes. This list is not exhaustive.

|                                                                                          | Chrome        | Safari       | Edge           | Firefox       | Brave        | Opera        | Tor          |
| ---------------------------------------------------------------------------------------- | ------------- | ------------ | -------------- | ------------- | ------------ | ------------ | ------------ |
| <a href="https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API">Canvas</a>         | ❌ Vulnerable | ⚠️ Flawed    | ❌ Vulnerable   | ⚠️ Flawed     | ✅ Resistant | ❌ Vulnerable | ✅ Resistant |
| <a href="https://developer.mozilla.org/en-US/docs/Web/API/OfflineAudioContext">Audio</a> | ❌ Vulnerable |              | ❌ Vulnerable   | ❌ Vulnerable | ✅ Resistant | ❌ Vulnerable | ✅ Resistant |

# Services & Projects

These are various fingerprinting services & projects, and their current effectiveness towards various browsers.

|                                                                | Chrome        | Safari       | Edge           | Firefox      | Brave        | Opera       | Tor          |
| -------------------------------------------------------------- | ------------- | ------------ | -------------- | ------------ | ------------ | ----------- | ------------ |
| <a href="https://fingerprint.com/demo">Fingerprint</a>         | ⚠️ Trackable  | ⚠️ Trackable | ⚠️ Trackable    | ⚠️ Trackable | ⚠️ Trackable | ⚠️ Trackable | ✅ Resistant |
| <a href="https://abrahamjuliot.github.io/creepjs/">CreepJS</a> | ⚠️ Trackable  | ✅ Resistant | ⚠️ Trackable    | ⚠️ Trackable | ⚠️ Trackable | ⚠️ Trackable | ✅ Resistant |
