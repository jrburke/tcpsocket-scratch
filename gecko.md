## Setup

Did an android setup:
https://wiki.mozilla.org/Mobile/Fennec/Android

For the ./mach mercurial-setup answered yes to all except for mqext to automatically
commit when making changes to a patch question.

## Geolocation

A changeset used as an entry point to find the code:
https://hg.mozilla.org/mozilla-central/rev/b54402f21eb8

dom/base/Navigator.cpp :: GetGeolocation, #include "nsGeolocation.h"
Navigator.h too

dom/geolocation/nsGeolocation.h
