# Reproducibility by any means necessary - lessons from MATLAB

A talk for the University of Sheffield Open Research Conversations, 20th November 2024.


## Using this repository
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/80x15.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.


## Rendering the slides locally
These slides are produced using [Quarto](https://quarto.org).

In order to render them locally, you will need to install Quarto from <https://quarto.org/docs/get-started/>.

Quarto documents can be rendered in either:
* VSCode
* RStudio (> 2022.07.1+554)
* Jupyter
* Terminal

Full instructions can be found at the link above, however in brief:
* In RStudio, open `index.qmd`, above the document click `Render`
* In the terminal, run `quarto render` to build the files, or `quarto preview` to spin up the preview server.

### Running MATLAB code cells

This presentation experimentally uses `mkernel` to run MATLAB code cells inside Quarto.

`mkernel` depends on `matlabengine` (the MATLAB engine for python), which is fun to install.

You may need to run the following commands from shell first, e.g. in Linux run the following, replacing `<matlabroot>` with the location of your MATLAB installation, e.g. `/usr/local/MATLAB/R2023a/`.

```sh
export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:<matlabroot>/bin/glnxa64
pip install matlabengine
```

```sh
pip install git+https://github.com/allefeld/mkernel.git
```

## Contributing
Contributions and improvements are very welcome! Please fork this repo and make a pull request against the `main` branch.
Please ensure that your document compiles successfully with the instructions above.