Jupyter notebook for deep learning example in LING 513 - this is based on an example from Matt Kelley's MoProc2019 Workshop Example. To open in binder, click on the binder badge next to the version you want.

LING 513 version: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/bvtucker/513_deep-learning-example.git/master)

# Instructions for running the notebook locally

These instructions will assume you have [already installed Julia](https://julialang.org/downloads/). They will also default you to using the latest version. If you would like to use the conference version, you will have to change branches on this page (in the upper left corner) before downloading, or change branches using Git if you use Git to clone the repository.

1. Install the appropriate packages in Julia:

  ```julia
] add Flux BSON Loess Plots ProgressBars Random Statistics IJulia
```

  The "]" at the beginning means to press the "]" key to enter the package interface. Copying the whole line of code including the "]" in the Julia REPL console should automatically enter the package interface as well.

2. Download this repository. If you use Git, this can be done using `git clone https://github.com/maetshju/moproc2019_deep_learning_workshop`. Otherwise, use the green "Clone or download" button at the upper right of the page.

3. Download and unzip the subset of the MALD data set that we will be working with. If you have access to a Bash console, you can run the "postBuild" script to automatically download and extract the files.

```bash
sh postBuild
```

  If not, download them from [the University of Alberta institutional repository](https://doi.org/10.7939/r3-b7v0-dy61). Make sure that the folder containing the MALD folders is placed in the same directory as the rest of the files in this repository.

4. Start a notebook in Julia. At the console interface:

  ```julia
using IJulia
notebook()
```

  Some information will be printed to the console, and a Jupyter notebook window will appear in your default web browser. If it asks you for a token, on a regular console (or CMD window on Windows), you will need to run `jupyter notebook list`, which will print out a URL with the token in it, which can be pasted into the webpage.

5. Use the Jupyter interface to find the corresponding "ipynb" files you downloaded as part of this repository. Clicking on them will open the notebooks, which you can then run from there.
