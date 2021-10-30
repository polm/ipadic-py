# ipadic-py

This is a version of IPAdic packaged for use in Python with
[mecab-python3](https://github.com/SamuraiT/mecab-python3) or
[fugashi](https://github.com/polm/fugashi). 

# You Shouldn't Use This

This is the version of IPAdic included with MeCab. It hasn't been updated since
at least 2007. The organization that created it no longer does this kind of
work. The contact URLs listed in the source no longer resolve. It doesn't
contain important recent terms like 令和, the current era name.

Instead you should use [Unidic](https://ccd.ninjal.ac.jp/unidic/), which is
maintained by NINJAL. 

This package is provided for compatability with old benchmarks or models.

## Usage

To install:

    pip install ipadic

To initialize with mecab-python3:

    import MeCab
    import ipadic
    tagger = MeCab.Tagger(ipadic.MECAB_ARGS)
    print(tagger.parse("図書館にいた事がバレた"))

# License

IPAdic is copyright the Nara Institute of Science and Technology and ICOT. For
details see the COPYING file included in this distribution. This version of the
dictionary is distributed in compliance with the terms specified in that file.

The code in this repository is by Paul McCann and is available under the MIT or
WTFPL license, as you prefer.
