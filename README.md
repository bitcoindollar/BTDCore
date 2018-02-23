Bitcoin Dollar Core integration/staging tree
=====================================

What is Bitcoin Dollar?
----------------

World's first artificial intelligence Bitcoin is a community-led project to create an experimental split
of blockchain ledger to a new proof-of-work and signature algorithm. The purpose for doing this is
to make Bitcoin mining decentralized again. Satoshi Nakamoto’s idealistic vision of “one CPU one
vote” has been superseded by a reality where the manufacture and distribution of mining equipment
has become dominated by a very small number of entities, some of whom have engaged in
abusive practices against individual miners and the Bitcoin network as a whole. Bitcoin Dollar will
provide an opportunity for countless new people around the world to participate in the mining
process with widely-available consumer hardware that is manufactured and distributed by reputable
mainstream corporations. A more decentralized, democratic mining infrastructure is more
resilient and more in line with Satoshi’s original vision. Perhaps, if the Bitcoin Dollar experiment is
judged by the community to be a success, it may one day help build consensus for a proof-of-work
and signature split on Bitcoin itself. 

For more information, as well as an immediately useable, binary version of
the Bitcoin Dollar Core software, see https://bitcoindollar.io/, or read the
[original whitepaper](https://goo.gl/sLjroR).

License
-------

Bitcoin Dollar Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/bitcoindollar/btd/tags) are created
regularly to indicate new official, stable release versions of Bitcoin Dollar Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

The developer [mailing list](https://lists.linuxfoundation.org/mailman/listinfo/bitcoindollar-dev)
should be used to discuss complicated or controversial changes before working
on a patch set.

Developer IRC can be found on Freenode at #bitcoin-core-dev.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](src/test/README.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`. Further details on running
and extending unit tests can be found in [/src/test/README.md](/src/test/README.md).

There are also [regression and integration tests](/test), written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/test) are installed) with: `test/functional/test_runner.py`

The system makes sure that every pull request is built for Windows, Linux, and OS X, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
------------


Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull would automatically overwrite them again.

Translators should also subscribe to the [mailing list](https://groups.google.com/forum/#!forum/bitcoindollar-translators).
