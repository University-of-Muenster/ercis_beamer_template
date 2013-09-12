# ERCIS beamer template

This repository maintains the sources of the [ERCIS](http://ercis.com/) presentation template for the LaTeX beamer package.

**Note for template users:** If you just intend to *use* the template to build a presentation, refer to the [releases section](./releases) on this GitHub page and download the latest version as an archive. You do not need to clone this repository unless you want to contribute to the template.

## System requirements
The following software is required to compile the template. In particular the build script requires the  ant and the pdflatex executables.
- [Apache Ant 1.9.2](http://ant.apache.org/)
- [TeX Live 2013](http://www.tug.org/texlive/)

Note: Older versions of the required software might also work, but have not tested.

## Building the template
In the root folder of the template, execute the following command to compile the template, the documentation and the example presentation. Afterwards, all generated files are available in the `dist` folder.

```
ant dist
```

Additionally, the generated files can be compressed to a single ZIP archive for publishing purposes. You can also find the resulting archive
```
ant package
```

The source files for the template reside in the `src` folder. During compilation, these source files are concatenated to the final template style `build/ercisbeamer.sty`. Therefore, changes have to be made in the source files in order to be incorporated into the template.

## Building a presentation
To build a presentation using the ERCIS beamer template, copy the templae style `build/ercisbeamer.sty` to the folder which contains your presentation and include it by `\usepackage{ercisbeamer}`. For details on using the template, refer to the corresponding section in the documentation.

## Contribution
Feel free to fork this repository and contribute error fixes, new features or other changes either using pull requests or direct contribution. In the case of questions, do not hesitate to contact me via [e-mail](mailto:dominik@lekse.de).
