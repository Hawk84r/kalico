# Contact

This document provides contact information for Kalico.
Kalico a community-maintained fork of the Kalico firmware.

## Discord

Kalico has a dedicated Discord server where you can chat with the 
developers and users of Kalico in real-time.

You can join the server here:
[kalico.gg/discord](https://kalico.gg/discord)

## I have a question about Kalico

Many questions we receive are already answered in the
[Overview](Overview.md). Please be sure to to read the
documentation and follow the directions provided there.

If you are interested in sharing your knowledge and experience with
other Kalico users then you can join the Kalico [Discord server](#discord)

If you have a general question or are experiencing general printing
problems, then also consider a general 3d-printing forum or a forum
dedicated to the printer hardware.

## I have a feature request

All new features require someone interested and able to implement that
feature. If you are interested in helping to implement or test a new
feature, you can search for ongoing developments on the 
[GitHub issues](https://github.com/KalicoCrew/kalico/issues) page and 
[pull requests](https://github.com/KalicoCrew/kalico/pulls) page

There also are discussions between collaborators on the Kalico [Discord server](#discord).

## Help! It doesn't work!

If you are experiencing problems we recommend you carefully read the
[Overview](Overview.md) and double check that all steps
were followed.

If you are experiencing a printing problem, then we recommend
carefully inspecting the printer hardware (all joints, wires, screws,
etc.) and verify nothing is abnormal. We find most printing problems
are not related to the Kalico software. If you do find a problem with
the printer hardware then consider searching general 3d-printing
forums or forums dedicated to the printer hardware.

## I found a bug in the Kalico software

Kalico is an open-source project and we appreciate when collaborators
diagnose errors in the software.

Problems should be reported on the [Discord server](#discord)

There is important information that will be needed in order to fix a
bug. Please follow these steps:
1. Make sure you are running unmodified code from
   [https://github.com/KalicoCrew/kalico](https://github.com/KalicoCrew/kalico).
   If the code has been modified or is obtained from another source,
   then you should reproduce the problem on the unmodified code from
   [https://github.com/KalicoCrew/kalico](https://github.com/KalicoCrew/kalico)
   prior to reporting.
2. If possible, run an `M112` command immediately after the
   undesirable event occurs. This causes Kalico to go into a
   "shutdown state" and it will cause additional debugging information
   to be written to the log file.
3. Obtain the Kalico log file from the event. The log file has been
   engineered to answer common questions the Kalico developers have
   about the software and its environment (software version, hardware
   type, configuration, event timing, and hundreds of other
   questions).
   1. Dedicated Kalico web interfaces have the ability to directly
      obtain the Kalico log file. It's the easiest way to obtain the
      log when using one of these interfaces. Otherwise, an "scp" or
      "sftp" utility is needed to copy the log file to your desktop
      computer. The "scp" utility comes standard with Linux and MacOS
      desktops. There are freely available scp utilities for other
      desktops (eg, WinSCP). The log file may be located in the
      `~/printer_data/logs/klippy.log` file (if using a graphical scp
      utility, look for the "printer_data" folder, then the "logs"
      folder under that, then the `klippy.log` file). The log file may
      alternatively be located in the `/tmp/klippy.log` file (if using
      a graphical scp utility that can not directly copy
      `/tmp/klippy.log` then repeatedly click on `..` or
      "parent folder" until reaching the root directory, click on
      the `tmp` folder, and then select the `klippy.log` file).
   2. Copy the log file to your desktop so that it can be attached to
      an issue report.
   3. Do not modify the log file in any way; do not provide a snippet
      of the log. Only the full unmodified log file provides the
      necessary information.
   4. It is a good idea to compress the log file with zip or gzip.
5. Open a new thread on the [Discord server](#discord)
   and provide a clear description of the problem. Other Kalico
   contributors will need to understand what steps were taken, what
   the desired outcome was, and what outcome actually occurred. The
   compressed Kalico log file should be attached to that topic.

## I am making changes that I'd like to include in Kalico

Kalico is open-source software and we appreciate new contributions.

See the [CONTRIBUTING document](CONTRIBUTING.md) for information.

There are several
[documents for developers](Overview.md#developer-documentation). If
you have questions on the code then you can also ask on the [Discord server](#discord)
