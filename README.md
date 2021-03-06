## Datatblr
##### Author: Johannes Schütt
##### Co-author: Claudia Saalbach

##### [Chair of Empirical Social Research Methods at the University of Potsdam](https://uni-potsdam.de/soziologie-methoden)

Datatblr is a program that generates a table collection with the univariate description of all metric and categorical variables in a dataset. Datatblr delivers a LaTeX and a pdf-document.

Datatblr is suitable for generating table volumes that typically appear in the appendix of research reports, or for the preparation of more detailed analysis.

### Dependencies
* R base (3.6.3 or newer)  [CRAN](https://cloud.r-project.org/)
  * [dplyr](https://cran.r-project.org/web/packages/dplyr/index.html) package
  * [rio](https://cran.r-project.org/web/packages/rio/index.html) package
* LaTeX [TeX Live](https://www.tug.org/texlive/)

#### To build the program:
* G++ compiler (std=c++17)
* Make

### Release

It is recommended that you download the latest **stable release** of the program. If you download the program from the master branch, there is a chance that the program may be unstable or not run at all.

### Build & Run
**UNIX:**
To build the Datatblr user interface, run the command

```shell
sh build.sh
```

inside the project folder. After that, you can run the executable by double-clicking on it or by running the command

```shell
./datatblr
```

You can move the executable as you like. Make sure to set your R working directory to `/path/to/Datatblr` **or** to move the `dtblr_core` folder into your own working directory. Your reports will be saved there.

You can set your working directory in your `.Rprofile` with this command:

```R
setwd("/path/to/working_directory")
```

You can also add the path of the executable to your PATH environment variable and then run the program using the command `datatblr`.

The user interface is compatible with UNIX systems. If you are running **Windows**, you have to work directly with the R files! (You might want to check out the lite version.)

### License
[GNU General Public License v2.0 only](https://github.com/johschuett/Datatblr/blob/master/GPL-2.0)

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
