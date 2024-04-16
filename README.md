# evhz

Show mouse refresh rate under linux + evdev

For information about polling rate, see https://wiki.archlinux.org/index.php/Mouse_Polling_Rate

Just do ./run (run is very short and readable).

Nonverbose mode = -n, but you probably don't want that.

Reported average is for the last 64 samples, or as many as we have so far.

There exists a kernel bug for USB ports which use the uhci_hcd driver,
where a 1000 hz mouse will only read at 500hz, causing jittering:
https://bugzilla.kernel.org/show_bug.cgi?id=60586. A workaround is to
use USB ports that use the ehci-pci driver.

Maintainer: Ian Kelling <ian@iankelling.org>

Bugs, patches, requests, feedback are welcome.


# license

I, Ian Kelling, follow the GNU license recommendations at
https://www.gnu.org/licenses/license-recommendations.en.html. They
recommend that small programs, < 300 lines, be licensed under the
Apache License 2.0. This file contains or is part of one or more small
programs.

Copyright 2024 Ian Kelling

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
