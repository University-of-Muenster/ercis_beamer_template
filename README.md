# ERCIS beamer template

This repository maintains the sources of the ERCIS template for the LaTeX beamer package.

## System requirements
The following software is required to compile the template.
- Java JDK 7
- Apache Ant 1.9.2

## Compile process
In the root folder of the template, run the following command to fully compile the template, the documentation and the example presentation. Afterwards, all generated files are available in the *dist* folder.

```
ant dist
```

Additionally, the generated files can be compressed to a single ZIP archieve for publishing purposes
```
ant package
```

## Source structure
The source files for the template reside in the *src* folder. During compilation, these source files are concatenated to the final template style *build/ercisbeamer.sty*. Therefore, changes have to be made in the source files in order to be incorporate into the template.

## Contribution
Feel free to fork this repository and contribute error fixes, new features or other changes using pull requests.
