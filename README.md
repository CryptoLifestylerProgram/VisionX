https://medium.com/@nrek/mac-os-x-10-11-ei-capitan%E4%B8%8B%E7%BC%96%E8%AF%91bitcoin%E6%BA%90%E4%BB%A3%E7%A0%81-1a30b8a1bc4a
VisionX Core 1.0.0
===============================

https://visionX.io


What is VisionX?
----------------

VisionX-Coin is a fully decentralised cryptocurrency built on the premise of providing anonymity, speed, fair mining by being ASIC-resistant and reliability by the usage of Masternodes.


For more information, as well as an immediately usable, binary version of
the VisionX Core software, see https://visionX.io


License
-------

VisionX Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is meant to be stable. Development is normally done in separate bran
[Tags](https://github.com/VisionX/VisionX/tags) are created to indicate new official,l.0.0
stable release versions of VisionX Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](/doc/unit-tests.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`

There are also [regression and integration tests](/qa) of the RPC interface, written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/qa) are installed) with: `qa/pull-tester/rpc-tests.py`

The Travis CI system makes sure that every pull request is built for Windows
and Linux, OS X, and that unit and sanity tests are automatically run.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

