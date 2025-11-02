# Galaxy-tutorials
A tutorial to understand the distributions of stars in our galaxy and their motions. This is a conglomerate of existing Astropy tutorials, and created as a part of Astro 1 course in TIFR in Fall 2025.

## Setup

To get started, first create a environment with the `galactut.yml` file. In your terminal, type the following: 

```markdown
#bash
conda env create -f galactut.yml
```
Once the environment is resolved and created successfully, to activate the galactut environment, run:

```markdown
#bash
conda activate galactut
```
Then in python or jupyter notebook opened in the environment, check

```markdown
#python
import numpy, scipy, astropy, gala, matplotlib, pandas
```
If imported successfully, we are halfway there. Next, check the versions: 

```markdown
#python
print("numpy:"numpy.__version__)
print("scipy:"scipy.__version__)
print("astropy:"astropy.__version__)
print("gala:"gala.__version__)
print("matplotlib:"matplotlib.__version__)
```
Make sure that your numpy version is < 2. If your gala version is less than <1.10.1 It might create some trouble in orbit calculation. In that case, in `galactut` environment run the following: 

```markdown
#bash
pip install --upgrade gala
```
And check the version in python: 
```markdown
#python
import gala
print("gala:"gala.__version__)
```
It should be 1.10.1, the latest stable version. 
