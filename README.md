macdict2
========

The second version of macdict.

Installation
------------

for Swift™ executable file:

> `make -f Makefile2 swfit`

for Objective-C executable file:

> `make -f Makefile2 objc`

Usage
-----

`macdict2 [-h] [-l] [-d <dictionary name>]... [-i <dictionary indexes>]... [word]...`

### Options: `-h`

Show help information and exit.

### Options: `-l`

Show a list of names of all available dictionaries with indexes.

### Options: `-d <dictionary>`

`dictionary` is the name of the dictionary.

If `dictionary` is `all`, then macdict2 will search all available dictionaries and show all the definitions of the word or phrase.

If no dictionary is specified, macdict2 will search all system built-in dictionaries and show the first definition found.

### Options: `-i <index>`

`index` is indexes of the dictionary delimited with commas `,`. If indexes contain `0` then all available dictionaries are selected.

This option is only recommended for a temporary use.

e.g.

```
$ macdict2 Quod Erat Demonstrandum
Definitions of <Quod Erat Demonstrandum>
quod erat demonstrandum |kwɒd ˌɛrat dɛmənˈstrandʊm | (abbrev.: QED) ▶exclamation used to convey that a fact or situation demonstrates the truth of one's theory or claim, especially to mark the conclusion of a formal proof. ORIGIN Latin, literally ‘which was to be demonstrated’.
```

```
$ macdict -d all Quod Erat Demonstrandum
Definitions of <Quod> in {Prisma woordenboek Nederlands}

quod |kwot| < Latijnvoornaamwoordwat, hetgeen~ erat demonstrandumhetgeen bewezen moest worden~ nonwat niet het geval is: als ik een nieuwe baan zou willen - ~ non - dan zou het iets in het onderwijs zijn~ licetwat toegestaan, geoorloofd is
%
Definitions of <Quod Erat Demonstrandum> in {スーパー大辞林}

Q.E.D.〖ラテン quod erat demonstrandum 〗「（このように）証明されるべきであったところの」の意。また，数学や物理で，「よって証明された」の意。
%
Definitions of <Quod Erat Demonstrandum> in {Oxford Dictionary of English}

quod erat demonstrandum |kwɒd ˌɛrat dɛmənˈstrandʊm | (abbrev.: QED) ▶exclamation used to convey that a fact or situation demonstrates the truth of one's theory or claim, especially to mark the conclusion of a formal proof. ORIGIN Latin, literally ‘which was to be demonstrated’.
%
Definitions of <Quod Erat Demonstrandum> in {New Oxford American Dictionary}

quod erat demonstrandum |kwäd ˈerət ˌdemənˈsträndəm | (abbr.: QED) ▶noun used to convey that a fact or situation demonstrates the truth of one's theory or claim, esp. to mark the conclusion of a formal proof. ORIGIN Latin, literally ‘which was to be demonstrated.’
%
Definitions of <Quod Erat Demonstrandum> in {New Ace English-Korean Dictionary and New Ace Korean-English Dictionary}

quod erat demonstrandum |kwɔ̀ːd érɑːt dèmənstrǽndəm, dèimɔːnstrɑ́ːndum|｛라틴어｝그 일은 증명되었어야 마땅했다.약어 Q.E.D.
```

```
macdict -d 'New Oxford American Dictionary' Quod Erat Demonstrandum
Definitions of <Quod Erat Demonstrandum> in {New Oxford American Dictionary}

quod erat demonstrandum |kwäd ˈerət ˌdemənˈsträndəm | (abbr.: QED) ▶noun used to convey that a fact or situation demonstrates the truth of one's theory or claim, esp. to mark the conclusion of a formal proof. ORIGIN Latin, literally ‘which was to be demonstrated.’
```

```
macdict -l                                                         
[1] Prisma woordenboek Nederlands
[2] スーパー大辞林
[3] Oxford Dictionary of English
[4] New Ace Korean Language Dictionary
[5] Oxford American Writer's Thesaurus
[6] New Oxford American Dictionary
[7] Multidictionnaire de la langue française
[8] New Ace English-Korean Dictionary and New Ace Korean-English Dictionary
[9] Diccionario General de la Lengua Española Vox
[10] ウィズダム英和辞典 / ウィズダム和英辞典
[11] 維基百科
[12] Oxford Thesaurus of English
[13] Oxford Chinese Dictionary
[14] Dizionario italiano da un affiliato di Oxford University Press
[15] Apple 辭典
```

- - -

macdict
=======

A commandline tool for Mac OS X to look up words in the builtin/user dictionaries.

Supports: OS X v10.5 and later

Installation
------------

for C executable file:

> `make c`

for Objective-C executable file:

> `make m`

for Python executable file:

> `make py`

for Shell executable file:

> `make sh`

Usage
-----

`macdict <words>`

e.g.

```
$ macdict Mac OS X
Definitions of <Mac OS X>
mac os
Mac OS
{Macintosh Operating System}

$ macdict 负增长
Definitions of <负增长>
负增长 fùzēngzhǎng 名词 negative growth 人口出现负增长。 The population appears to be in decline.
```
