This is a personal fork of bootstrap.  It includes the following changes
from upstream:

---

## Additional Breakpoints:

Bootstrap claims to be 'mobile first'.  Realistically, it's actually
mobile-only.  The largest breakpoint they provide is at 1200 pixels,
which means that if you want to do any kind of responsive behavior other
than just generic stuff on any modern desktop or workstation displays
(or televisions, or any number of other big displays), you need to do
some custom CSS, which may not integrate well with Bootstrap.

This fork  adds the following additonal breakpoints so custom CSS
shouldn't be needed, and things Just Work (TM):

* `hd`: Breaks at 1280 pixels (HD width, also called 720p).
* `fhd`: Breaks at 1920 pixels (Full HD width, also called 1080p).
* `qhd`: Breaks at 2560 pixels (Quad HD width, sometimes called 2k or 1440p).
* `uhd1`: Breaks at 3840 pixels (4k UHD-1 width, also called 2160p).
* `uhd2`: Breaks at 7680 pixels (8k UHD-2 width, also called 4320p).

The original breakpoints are still present, and are expected to be used
for mobile layouts.  The upstream `xl` breakpoint is approximately the
same size as the `hd` breakpoint, so it's generally better to use one
or the other, not both.

The additional breakpoints are also extended to the modal functionality,
providing `modal-hd` through `modal-uhd2` classes that will scale up to
fill equivalently sized screens.

----

The upstream README can be found in README.upstream.md.
