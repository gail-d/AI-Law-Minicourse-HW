# AI-Law-Minicourse-HW1
# Step 1 :white_square_button:

```
 #Import Scientific Packages into Python Kernel
from bs4 import BeautifulSoup 
import requests 
import re 

import pandas as pd
import numpy as np

 #Set a user-agent in your header so you aren't flagged by the browser when making an HTTP request
headers = {'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) \
           Chrome/39.0.2171.95 Safari/537.36'}
``` 

## Step 1.1:
If you aren’t in the “right” directory when running jupyter notebook, an error is returned saying you don’t have the correct modules installed.  While uncertain what numpy, panda and beautiful soup do, they apparently were found.  And, the dict variable “headers” is a size 240 and set to {'User-Agent': 'Chrome/39.0.2171.95'}.  It is likely that the headers variable  - user agent is a library that identifies a device and allows you to operate in your respective browser.  There was no output. This didn’t actually load on a Mac, most likely because the “bs4” and “BeautifulSoup” folders or packages do not exist locally or in my cloned spaces. We’re wondering if this is specific to a particular OS or virtual machine setup since it works on a local space setup. 

```
#Link url from caselaw which has a repository of Supreme Court ruling opinions and assign to variable
root_url = "http://caselaw.findlaw.com/court/us-supreme-court/years/"
```

## Step 1.2:
We do not see the images as indicated in the slide presentation. However, the string variable root-url was created, size = 105, value =  http://caselaw.findlaw.com/court/us-supreme-court/years/.  There was no output.

### Step 1.3.1:
This step creates a list called “years” with an undefined limit to the variable, and its size is 2216.  There was no output.

### Step 1.3.2:
This step likely doe create a truncated name for a function - as it is not a variable, we do not have information regarding it.  And, there is no output for this function.

### Step 1.3.3:
The df DataFrame variable was created of size 374368.  We are completely clueless as to its design.  We are assuming it is building the data set; however, this is the sole output:

```
E:\Programs\Anaconda\lib\site-packages\ipykernel_launcher.py:2: DeprecationWarning: 
.ix is deprecated. Please use
.loc for label based indexing or
.iloc for positional indexing

See the documentation here:
http://pandas.pydata.org/pandas-docs/stable/indexing.html#ix-indexer-is-deprecated
 
Out[12]: 'http://caselaw.findlaw.com/us-supreme-court/05-1101.html'
```

## Step 1. End
Successfully produced the array size of (23393, 2). This array shape tells us that we’re set up for 23 thousand court cases. 
:thumbsup:

# Step 2 :white_square_button:
## Step 2.1
Even though bs4 and pandas were previously loaded, we reloaded them as per the example. It looks like the supcourt definition is created to limit the number of requests that we make to the caselaw website. Supcourt, test_df, test2_df and test3_df are al DataFrame variables with varying sizes.  There is no output.  


## Step 2.2
We can now see that we’ve been building a database and the mechanisms to view that database. At this point, we understand ***why*** we haven’t received any output or explanations for the code we’re writing. We have hashed explanations in the code that describe the literal effects of the code, but no overall explanation for what we’re creating or should be seeing. 


# Step 3 :white_square_button:
We’re not sure if this worked, since no new variables were created and no error messages displayed. Without any direction in these tutorials, we can only assume (as we have for the past 2 steps) that what we’re doing is correct. The add-on Variable inspector was invaluable in helping us determine that we actually were in the process of creating something. Common words are theoretically assigned.

# Step 4 :white_square_button:
We don’t see the  printout that is displayed after some of the steps here. But, as in the previous step, we are not getting any error messages. Also, it’s not clear whether we should be seeing the printouts that are interspersed in the tutorial or if those images are for reference. 

-------------
# TENSORFLOW :white_square_button: 
### We were able to recreate the tensorflow example. :thumbsup: 
```
E:\Programs\Anaconda\lib\site-packages\h5py\__init__.py:34: FutureWarning: Conversion of the second argument of issubdtype from `float` to `np.floating` is deprecated. In future, it will be treated as `np.float64 == np.dtype(float).type`.
 from ._conv import register_converters as _register_converters

Found and verified text8.zip
Data size 17005207
Most common words (+UNK) [['UNK', 418391], ('the', 1061396), ('of', 593677), ('and', 416629), ('one', 411764)]
Sample data [5234, 3081, 12, 6, 195, 2, 3134, 46, 59, 156] ['anarchism', 'originated', 'as', 'a', 'term', 'of', 'abuse', 'first', 'used', 'against']
3081 originated -> 5234 anarchism
3081 originated -> 12 as
12 as -> 6 a
12 as -> 3081 originated
6 a -> 12 as
6 a -> 195 term
195 term -> 6 a
195 term -> 2 of
Initialized
Average loss at step  0 :  256.35723876953125
Nearest to it: limbo, eerie, dad, ataxia, emergence, acacias, hiker, esteem,
Nearest to no: toledo, clearer, ransom, debugging, bosman, capping, plane, symbolics,
Nearest to up: autoimmune, crewmembers, armando, da, autographed, carnot, salting, ship,
Nearest to however: polk, marca, lac, hedonist, swivel, familia, corridors, sedatives,
Nearest to called: thymus, civilized, cpk, debuted, haldane, compression, philibert, prostaglandins,
Nearest to most: deficiencies, palaces, vasily, pcc, vo, ideological, pakistan, observable,
Nearest to war: vonnegut, disney, transonic, brothel, meticulous, promenade, xxv, rates,
Nearest to used: sven, lorica, trujillo, anthropologist, mit, hort, beads, chalk,
Nearest to as: ceiba, marcius, mutagens, cooperates, furthered, countless, manager, digs,
Nearest to five: halley, modalities, collingwood, omim, disproven, bar, descend, wrinkled,
Nearest to such: kilo, creams, nami, acc, landmines, quantity, gaba, fasts,
Nearest to see: hades, mic, cause, rhodope, glastonbury, seeming, lippincott, electro,
Nearest to state: engined, consanguinity, lenient, printer, linguist, minicomputers, im, mobilization,
Nearest to these: mediaeval, overridden, symmetry, nanyang, maintaining, nikita, golfo, kiritimati,
Nearest to between: trax, jaffe, abies, variance, newsreels, arco, assam, surveying,
Nearest to and: poisoned, fiesole, omri, utterances, pessimism, pasta, seniority, dramatists,
Average loss at step  2000 :  113.36779870414733
Average loss at step  4000 :  53.12698460841179
Average loss at step  6000 :  33.28791245150566
Average loss at step  8000 :  23.73432744169235
Average loss at step  10000 :  17.749609692811966
Nearest to it: he, ataxia, wilmot, encyclopaedia, limbo, cube, this, faso,
Nearest to no: phi, ransom, toledo, plane, mechanism, indonesia, refrigerator, blackwell,
Nearest to up: likely, ignosticism, ship, da, accessed, biscuit, boxes, perform,
Nearest to however: polk, lymphoma, host, cosmonaut, walked, soul, solf, bckgr,
Nearest to called: civilized, debuted, allies, easily, put, pregnancy, shield, unknown,
Nearest to most: yeast, pakistan, archie, UNK, investigations, gogh, palaces, confuse,
Nearest to war: coke, aries, disney, meticulous, hierarchy, rates, declared, discovery,
Nearest to used: beads, gland, throne, commanded, complete, hort, ionian, connor,
Nearest to as: and, in, is, to, was, of, archie, by,
Nearest to five: gland, halley, nine, zero, agave, pace, archie, three,
Nearest to such: output, inherently, themed, mozambique, a, congo, conquered, line,
Nearest to see: cause, lm, hieroglyphic, six, glastonbury, hades, inorganic, precision,
Nearest to state: capitalism, jpg, engined, im, oil, series, wires, moulds,
Nearest to these: worth, tar, maintaining, drop, interpretation, gabriel, discovered, kinds,
Nearest to between: and, basins, UNK, variance, alien, surveying, zero, earl,
Nearest to and: of, in, or, UNK, to, with, gland, as,
Average loss at step  12000 :  14.12494773375988
Average loss at step  14000 :  11.878604223489761
Average loss at step  16000 :  9.878924388885498
Average loss at step  18000 :  8.318806460142136
Average loss at step  20000 :  7.92748183965683
Nearest to it: he, this, they, which, encyclopaedia, the, and, not,
Nearest to no: toledo, phi, debugging, now, windsor, meridians, ransom, plane,
Nearest to up: likely, ignosticism, carnot, sar, perform, accessed, ship, retail,
Nearest to however: polk, familia, three, solf, soul, photoshop, lymphoma, cosmonaut,
Nearest to called: civilized, easily, debuted, prostaglandins, UNK, unknown, hein, shield,
Nearest to most: yeast, dasyprocta, pakistan, agouti, selector, deficiencies, accomplished, investigations,
Nearest to war: coke, aries, disney, rates, meticulous, discovery, hierarchy, synod,
Nearest to used: operatorname, truetype, hort, antwerp, throne, ionian, dasyprocta, gland,
Nearest to as: and, is, agouti, was, onyx, in, by, dasyprocta,
Nearest to five: nine, zero, six, eight, seven, three, two, four,
Nearest to such: evangelist, latinus, mozambique, output, circ, the, yale, themed,
Nearest to see: cause, lm, and, operatorname, precision, glastonbury, bartlett, six,
Nearest to state: capitalism, wires, dasyprocta, major, operatorname, moulds, kay, nursing,
Nearest to these: symmetry, gabriel, drop, worth, tar, aversion, maintaining, the,
Nearest to between: and, basins, in, with, of, from, surveying, zero,
Nearest to and: or, agouti, in, of, circ, operatorname, dasyprocta, for,
Average loss at step  22000 :  7.015894997119903
Average loss at step  24000 :  6.866622223854065
Average loss at step  26000 :  6.725065308630467
Average loss at step  28000 :  6.359819702386856
Average loss at step  30000 :  5.942696993231773
Nearest to it: he, this, which, there, they, birkenau, not, abet,
Nearest to no: toledo, birkenau, now, windsor, phi, a, meridians, debugging,
Nearest to up: likely, sar, binds, dimensionless, carnot, ignosticism, caterpillars, accessed,
Nearest to however: but, three, polk, solf, and, photoshop, six, familia,
Nearest to called: civilized, prostaglandins, easily, birkenau, debuted, see, UNK, and,
Nearest to most: yeast, dasyprocta, pakistan, agouti, deficiencies, accomplished, palaces, investigations,
Nearest to war: abet, coke, disney, meticulous, aries, rates, discovery, hierarchy,
Nearest to used: operatorname, truetype, hort, antwerp, ionian, nocturnal, gland, dasyprocta,
Nearest to as: agouti, and, by, onyx, is, dasyprocta, steiner, speedup,
Nearest to five: six, eight, four, seven, zero, nine, three, two,
Nearest to such: evangelist, latinus, yale, mozambique, circ, acc, themed, output,
Nearest to see: and, networked, ansgar, cause, precision, operatorname, abused, lm,
Nearest to state: wires, capitalism, major, dasyprocta, kay, operatorname, series, moulds,
Nearest to these: symmetry, gabriel, drop, the, tar, nikita, vigilance, mut,
Nearest to between: with, from, in, basins, into, surveying, shipping, variance,
Nearest to and: or, agouti, circ, operatorname, dasyprocta, birkenau, in, but,
Average loss at step  32000 :  5.965334744811058
Average loss at step  34000 :  5.704222206234932
Average loss at step  36000 :  5.800072292327881
Average loss at step  38000 :  5.500229636907577
Average loss at step  40000 :  5.248446915864944
Nearest to it: he, this, which, there, they, that, maxi, not,
Nearest to no: a, birkenau, toledo, now, meridians, windsor, phi, three,
Nearest to up: banzer, likely, binds, dimensionless, sar, accessed, child, carnot,
Nearest to however: but, polk, and, solf, photoshop, minuet, gregorian, familia,
Nearest to called: UNK, civilized, prostaglandins, see, easily, birkenau, debuted, arexx,
Nearest to most: dasyprocta, yeast, agouti, pakistan, deficiencies, accomplished, more, vma,
Nearest to war: abet, meticulous, rates, coke, disney, aries, hierarchy, turbo,
Nearest to used: operatorname, bjarne, hort, gland, truetype, antwerp, dasyprocta, ionian,
Nearest to as: agouti, speedup, dasyprocta, and, onyx, is, steiner, by,
Nearest to five: six, four, eight, seven, zero, three, two, nine,
Nearest to such: well, evangelist, yale, mozambique, known, latinus, circ, radcliffe,
Nearest to see: networked, ansgar, cause, operatorname, precision, abused, called, lm,
Nearest to state: capitalism, wires, dasyprocta, kay, major, operatorname, albury, series,
Nearest to these: which, symmetry, drop, gabriel, mut, matters, nikita, vigilance,
Nearest to between: with, in, from, into, basins, surveying, and, at,
Nearest to and: or, agouti, circ, in, operatorname, but, zero, birkenau,
Average loss at step  42000 :  5.353010960817337
Average loss at step  44000 :  5.253884016871452

Average loss at step  46000 :  5.22815080666542
Average loss at step  48000 :  5.284570249199867
Average loss at step  50000 :  4.998463729858399
Nearest to it: he, this, there, which, they, kapoor, maxi, she,
Nearest to no: a, birkenau, toledo, now, windsor, meridians, three, leaped,
Nearest to up: banzer, binds, him, child, likely, accessed, dimensionless, caterpillars,
Nearest to however: but, and, when, solf, agouti, photoshop, circ, minuet,
Nearest to called: easily, and, prostaglandins, see, civilized, vma, UNK, gland,
Nearest to most: more, dasyprocta, yeast, agouti, accomplished, pakistan, gigantopithecus, deficiencies,
Nearest to war: abet, brothel, meticulous, rates, disney, scharnhorst, coke, hierarchy,
Nearest to used: operatorname, kapoor, bjarne, gland, ionian, hort, nocturnal, render,
Nearest to as: agouti, speedup, dasyprocta, onyx, is, eight, trinomial, by,
Nearest to five: six, four, three, seven, eight, two, zero, operatorname,
Nearest to such: well, known, radcliffe, yale, evangelist, circ, mozambique, latinus,
Nearest to see: networked, called, cause, abused, ansgar, precision, and, inorganic,
Nearest to state: major, kapoor, wires, capitalism, kay, dasyprocta, affiliated, series,
Nearest to these: some, which, all, drop, gabriel, kapoor, mut, vigilance,
Nearest to between: in, with, from, into, three, basins, through, surveying,
Nearest to and: or, but, agouti, circ, operatorname, four, birkenau, six,
Average loss at step  52000 :  5.037992403864861
Average loss at step  54000 :  5.185121445417404
Average loss at step  56000 :  5.044133465528488
Average loss at step  58000 :  5.052556781291962
Average loss at step  60000 :  4.968019167423249
Nearest to it: he, this, there, which, michelob, they, she, ursus,
Nearest to no: a, birkenau, debugging, meridians, now, toledo, windsor, leaped,
Nearest to up: him, binds, accessed, banzer, child, dimensionless, elegy, caterpillars,
Nearest to however: but, minuet, when, solf, three, ursus, agouti, circ,
Nearest to called: prostaglandins, UNK, see, easily, civilized, vma, and, gland,
Nearest to most: more, dasyprocta, agouti, yeast, deficiencies, gigantopithecus, many, accomplished,
Nearest to war: abet, rates, brothel, scharnhorst, meticulous, turbo, disney, coke,
Nearest to used: michelob, operatorname, microsite, kapoor, gland, known, hort, render,
Nearest to as: agouti, speedup, in, dasyprocta, onyx, and, by, steiner,
Nearest to five: four, six, three, eight, seven, nine, two, zero,
Nearest to such: well, known, yale, radcliffe, circ, creams, evangelist, ilya,
Nearest to see: abused, and, called, networked, precision, ansgar, cause, inorganic,
Nearest to state: kapoor, major, ursus, wires, dasyprocta, capitalism, michelob, kay,
Nearest to these: some, all, many, which, three, gabriel, two, mut,
Nearest to between: with, in, from, into, through, basins, surveying, under,
Nearest to and: or, ursus, but, agouti, circ, operatorname, birkenau, kapoor,
Average loss at step  62000 :  5.001193501353264
Average loss at step  64000 :  4.8314538549780845
Average loss at step  66000 :  4.611407443642617
Average loss at step  68000 :  4.9757218797206875
Average loss at step  70000 :  4.910627064347267
Nearest to it: he, this, there, which, she, they, michelob, ursus,
Nearest to no: a, birkenau, debugging, any, toledo, meridians, now, windsor,
Nearest to up: him, binds, accessed, banzer, child, caterpillars, kapoor, dimensionless,
Nearest to however: but, minuet, when, manchus, although, though, solf, and,
Nearest to called: easily, UNK, prostaglandins, see, vma, apprentices, gland, lifted,
Nearest to most: more, dasyprocta, agouti, some, schwa, yeast, many, deficiencies,
Nearest to war: abet, rates, brothel, upanija, scharnhorst, turbo, meticulous, synod,
Nearest to used: michelob, operatorname, microsite, cebus, kapoor, gland, known, dasyprocta,
Nearest to as: agouti, upanija, speedup, dasyprocta, thaler, honeycomb, trinomial, timecode,
Nearest to five: four, six, three, eight, seven, nine, two, zero,
Nearest to such: well, known, radcliffe, yale, these, ilya, circ, many,
Nearest to see: abused, thaler, ansgar, called, networked, but, precision, agouti,
Nearest to state: kapoor, major, wires, dasyprocta, michelob, ursus, kay, agouti,
Nearest to these: some, all, which, many, several, such, mut, gabriel,
Nearest to between: with, in, from, into, through, basins, surveying, under,
Nearest to and: or, ursus, but, circ, agouti, birkenau, operatorname, kapoor,
Average loss at step  72000 :  4.756143835425377
Average loss at step  74000 :  4.79828647005558
Average loss at step  76000 :  4.7268058506250386
Average loss at step  78000 :  4.791068026721478
Average loss at step  80000 :  4.825029657125473
Nearest to it: he, this, there, she, which, michelob, they, ursus,
Nearest to no: a, birkenau, debugging, any, toledo, now, meridians, windsor,
Nearest to up: him, binds, accessed, carnot, banzer, caterpillars, child, them,
Nearest to however: but, when, minuet, though, although, manchus, cebus, thaler,
Nearest to called: see, vma, easily, prostaglandins, gland, apprentices, lifted, kosar,
Nearest to most: more, some, dasyprocta, many, schwa, yeast, agouti, deficiencies,
Nearest to war: abet, brothel, crb, rates, turbo, meticulous, scharnhorst, vijay,
Nearest to used: michelob, known, operatorname, cebus, microsite, kapoor, gland, dasyprocta,
Nearest to as: agouti, dasyprocta, upanija, speedup, onyx, trinomial, thaler, microcebus,
Nearest to five: four, six, seven, three, eight, nine, two, zero,
Nearest to such: well, known, these, radcliffe, yale, many, ilya, circ,
Nearest to see: called, abused, thaler, agouti, but, courtly, operatorname, precision,
Nearest to state: kapoor, wires, major, dasyprocta, michelob, ursus, kay, printer,
Nearest to these: some, which, many, all, such, several, mut, gabriel,
Nearest to between: with, in, from, into, through, basins, surveying, under,
Nearest to and: or, but, ursus, iit, operatorname, birkenau, agouti, circ,
Average loss at step  82000 :  4.764839336156845
Average loss at step  84000 :  4.772643937706947
Average loss at step  86000 :  4.766079961419106
Average loss at step  88000 :  4.750964236140251
Average loss at step  90000 :  4.73619971048832
Nearest to it: he, this, there, she, they, michelob, which, maxi,
Nearest to no: a, any, birkenau, now, meridians, debugging, toledo, lone,
Nearest to up: him, binds, them, accessed, aquilegia, child, carnot, caterpillars,
Nearest to however: but, and, although, when, minuet, cebus, though, that,
Nearest to called: see, vma, prostaglandins, UNK, gland, kosar, easily, apprentices,
Nearest to most: more, some, many, schwa, dasyprocta, yeast, less, agouti,
Nearest to war: abet, crb, brothel, upanija, turbo, rates, scharnhorst, meticulous,
Nearest to used: michelob, known, cebus, operatorname, kapoor, microsite, gland, dasyprocta,
Nearest to as: agouti, dasyprocta, upanija, by, speedup, onyx, thaler, and,
Nearest to five: seven, four, eight, six, three, zero, nine, two,
Nearest to such: well, these, known, radcliffe, yale, including, circ, ilya,
Nearest to see: but, called, agouti, and, courtly, abused, thaler, operatorname,
Nearest to state: kapoor, dasyprocta, wires, michelob, ursus, agouti, iit, major,
Nearest to these: some, which, all, many, such, several, they, their,
Nearest to between: with, in, from, into, through, under, basins, surveying,
Nearest to and: or, but, ursus, iit, birkenau, circ, agouti, operatorname,
Average loss at step  92000 :  4.663192920684814
Average loss at step  94000 :  4.716123922944069
Average loss at step  96000 :  4.684394029855728
Average loss at step  98000 :  4.604774296164512
Average loss at step  100000 :  4.694002783179283
Nearest to it: he, this, there, she, they, michelob, which, ursus,
Nearest to no: any, a, birkenau, meridians, lone, rgya, debugging, now,
Nearest to up: him, them, binds, out, accessed, aquilegia, caterpillars, child,
Nearest to however: but, although, that, though, minuet, when, cebus, and,
Nearest to called: UNK, see, vma, apprentices, prostaglandins, kosar, autocorrelation, gland,
Nearest to most: more, some, many, schwa, dasyprocta, yeast, less, agouti,
Nearest to war: abet, brothel, upanija, crb, turbo, meticulous, vijay, rates,
Nearest to used: known, michelob, cebus, operatorname, kapoor, microsite, gland, dasyprocta,
Nearest to as: agouti, dasyprocta, upanija, speedup, thaler, onyx, microcebus, stenella,
Nearest to five: four, seven, six, three, eight, two, nine, zero,
Nearest to such: well, known, these, yale, including, many, radcliffe, circ,
Nearest to see: but, agouti, courtly, thaler, abused, operatorname, called, list,
Nearest to state: kapoor, wires, michelob, dasyprocta, ursus, building, iit, city,
Nearest to these: some, many, which, all, such, several, their, they,
Nearest to between: with, in, from, abies, through, into, under, constituci,
Nearest to and: or, but, iit, circ, ursus, operatorname, birkenau, agouti,
```
