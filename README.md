# Browser Fingerprinting Resistance Research (Work in Progress)

This repo is a summary of current <a href="https://en.wikipedia.org/wiki/Device_fingerprint#Browser_fingerprint">browser fingerprinting</a> protections used by various browsers and their effectiveness against various fingerprinting techniques & services.

# Techniques

These are known fingerprinting techniques & each browser's susceptibility to each for tracking purposes. This list is not exhaustive.

| | Chrome | Safari | Edge | Firefox | <a href="https://brave.com/">Brave</a> | Opera | <a href="https://www.torproject.org/">Tor</a> / <a href="https://mullvad.net/en/browser">Mullvad<a> |
| ------------------------------------------------------------------------------------------------------------------ | ------------- | ------------ | -------------- | ------------- | ------------ | ------------ | ------------ |
| <a href="https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API">Canvas API</a>                               | ❌ Vulnerable | ✅ Resistant | ❌ Vulnerable   | ✅ Resistant  | ✅ Resistant | ❌ Vulnerable | ✅ Resistant |
| <a href="https://developer.mozilla.org/en-US/docs/Web/API/OffscreenCanvas">OffscreenCanvas</a>                     | ❌ Vulnerable | ⚠️ <a href="https://github.com/Joe12387/safari-canvas-fingerprinting-exploit">Flawed</a> | ❌ Vulnerable   | ⚠️ <a href="https://bugzilla.mozilla.org/show_bug.cgi?id=1885471">Flawed</a> | ✅ Resistant | ❌ Vulnerable | ✅ Resistant |
| <a href="https://developer.mozilla.org/en-US/docs/Web/API/AudioContext">AudioContext</a>                           | ❌ Vulnerable | ⚠️ <a href="https://fingerprint.com/blog/bypassing-safari-17-audio-fingerprinting-protection/">Flawed</a> | ❌ Vulnerable   | ❌ Vulnerable | ✅ Resistant | ❌ Vulnerable | ✅ Disabled |
| <a href="https://developer.mozilla.org/en-US/docs/Web/API/OfflineAudioContext">OfflineAudioContext</a>             | ❌ Vulnerable | ⚠️ <a href="https://fingerprint.com/blog/bypassing-safari-17-audio-fingerprinting-protection/">Flawed</a> | ❌ Vulnerable   | ❌ Vulnerable | ✅ Resistant | ❌ Vulnerable | ✅ Disabled |
| <a href="https://developer.mozilla.org/en-US/docs/Web/API/WebGLProgram">WebGLProgram</a>                           | ❌ Vulnerable | ✅ Resistant | ❌ Vulnerable   | ❌ Vulnerable | ✅ Resistant | ❌ Vulnerable | ✅ Disabled |
| <a href="https://developer.mozilla.org/en-US/docs/Web/API/WEBGL_debug_renderer_info">WEBGL_debug_renderer_info</a> | ❌ Vulnerable | ✅ Resistant | ❌ Vulnerable   | ❌ Vulnerable | ✅ Resistant | ❌ Vulnerable | ✅ Disabled |
| <a href="https://github.com/brave/brave-browser/issues/24681">Timing Resolution</a>                                | ❌ Vulnerable | ✅ Unaffected | ❌ Vulnerable   | ✅ Unaffected | ✅ Resistant | ❌ Vulnerable | ✅ Unaffected |
| <a href="https://developer.mozilla.org/en-US/docs/Web/API/Navigator/hardwareConcurrency">hardwareConcurrency</a>  | ❌ Vulnerable | ✅ Resistant | ❌ Vulnerable   | ❌ Vulnerable   | ✅ Resistant | ❌ Vulnerable | ✅ Resistant |
| <a href="https://developer.mozilla.org/en-US/docs/Web/API/Navigator/deviceMemory">deviceMemory</a>                | ❌ Vulnerable | ✅ Unaffected | ❌ Vulnerable   | ✅ Unaffected   | ✅ Resistant | ❌ Vulnerable | ✅ Unaffected |
| <a href="https://developer.mozilla.org/en-US/docs/Web/API/Navigator/doNotTrack">doNotTrack</a>                    | ❌ Vulnerable | ✅ Unaffected | ❌ Vulnerable   | ❌ Vulnerable   | ✅ Resistant | ❌ Vulnerable | ✅ Resistant |
| Font Detection                                                                                                    | ❌ Vulnerable | ✅ Resistant  | ❌ Vulnerable   | ❌ Vulnerable   | ✅ Resistant | ❌ Vulnerable | ✅ Resistant |
| <a href="https://developer.mozilla.org/en-US/docs/Web/API/Window/screen">screen</a>                               | ❌ Vulnerable | ✅ Resistant  | ❌ Vulnerable   | ❌ Vulnerable   | ❌ Vulnerable | ❌ Vulnerable | ✅ Resistant |
| <a href="https://developer.mozilla.org/en-US/docs/Web/API/Performance/memory">jsHeapSizeLimit</a>                 | ❌ Vulnerable | ✅ Unaffected | ❌ Vulnerable   | ✅ Unaffected   | ❌ Vulnerable | ❌ Vulnerable | ✅ Unaffected |
| <a href="https://developer.mozilla.org/en-US/docs/Web/API/WebRTC_API">WebRTC</a>                                  | ❌ Vulnerable | ❌ Vulnerable | ❌ Vulnerable   | ❌ Vulnerable   | ❌ Vulnerable | ❌ Vulnerable | ✅ Disabled |

Updated: Sun, Mar 17, 2024

# Services & Projects

These are various fingerprinting services & projects, and their current effectiveness towards various browsers.

| | Chrome | Safari | Edge | Firefox | <a href="https://brave.com/">Brave</a> | Opera | <a href="https://www.torproject.org/">Tor</a> / <a href="https://mullvad.net/en/browser">Mullvad<a> |
| --------------------------------------------------------------------- | ------------- | ------------ | ----------- | ------------ | ------------ | ----------- | ------------- |
| <a href="https://fingerprint.com/demo">Fingerprint</a>                | ⚠️ Trackable  | ⚠️ Trackable | ⚠️ Trackable | ⚠️ Trackable | ⚠️ Trackable | ⚠️ Trackable | ✅ Resistant  |
| <a href="https://abrahamjuliot.github.io/creepjs/">CreepJS</a>        | ⚠️ Trackable  | ✅ Resistant | ⚠️ Trackable | ⚠️ Trackable | ⚠️ Trackable | ⚠️ Trackable | ✅ Resistant  |
| <a href="https://www.snowcatcloud.com/fingerprint/">Snowcat Cloud</a> | ⚠️ Trackable  | ⚠️ Trackable | ⚠️ Trackable | ⚠️ Trackable | ⚠️ Trackable | ⚠️ Trackable | ✅ Resistant? |

Updated: Wed, Apr 17, 2024
