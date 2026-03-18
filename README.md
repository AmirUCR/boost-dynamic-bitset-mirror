# Boost Mirror

This repo is a dependency for ALLEGRO. Steps to reproduce:

1. Download Boost from https://www.boost.org/releases/latest/ (I downloaded boost_1_90_0.tar.gz)
1. Unzip it `tar -xvzf boost_1_90_0.tar.gz `
1. `cd boost_1_90_0/`
1. `chmod +x ./bootstrap.sh`
1. `./bootstrap.sh`
1. `./b2 tools/bcp`
1. Then, run BCP, (https://www.boost.org/doc/libs/1_40_0/tools/bcp/bcp.html) to "rip" out the dynamic bitset header-only library
    ```
    ./dist/bin/bcp dynamic_bitset ../boost-dynamic-bitset-mirror
    ```
1. Delete anything that is not `boost/`, `LICENSE_1_0.txt`, and `README.md`

# Boost C++ Libraries

The Boost project provides free peer-reviewed portable C++ source libraries.

We emphasize libraries that work well with the C++ Standard Library. Boost
libraries are intended to be widely useful, and usable across a broad spectrum
of applications. The Boost license encourages both commercial and non-commercial use
and does not require attribution for binary use. 

The project website is www.boost.org, where you can obtain more information and
[download](https://www.boost.org/users/download/) the current release.
