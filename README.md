# jump-start-with-git-tian47720
jump-start-with-git-tian47720 created by GitHub Classroom
1、Quitting from lines 223-235 (Introduction.Rmd) 
Error in library(dplyr) :
Some errors like these, it means a lack of packages. Using 'install.packages()' to solve it. The packages I installed are "dplyr","sessioninfo","lobstr","sloop","RSQLite","zeallot","profvis","bench","ggbeeswarm".
2、The following objects are masked from 'package:stats': filter, lag
The following objects are masked from 'package:base':intersect, setdiff, setequal, union
contributors <- read.csv("contributors.csv", stringsAsFactors = FALSE,encoding = "UTF-8")
3、Quitting from lines 96-103 (Functionals.Rmd) 
Error in loadNamespace(name) : �����ڽ�'emo'������ֵĳ̼���
Calls: local ... loadNamespace -> withRestarts -> withOneRestart -> doWithOneRestart
We can restart Rstudio, and  step on 
> library(usethis)
> library(devtools)
> devtools::install_github("hadley/emo")
> devtools::install_github("hadley/sloop")
4、Warning message:
In system(cmd) : 'make' not found
Quitting from lines 77-84 (Rcpp.Rmd) 
Error in sourceCpp(code = code, env = env, rebuild = rebuild, cacheDir = cacheDir,  : 
  Error 1 occurred building shared library.
Calls: local ... withVisible -> eval -> eval -> cppFunction -> sourceCpp
We can install rtools to C，and add it to path. Then we execute the command in git and restart Rstudio
$git config --global http.sslBackend "openssl"
$git config --global http.sslCAInfo “D:\Git\mingw64\ssl\cert.pem”
5、����: LaTeX failed to compile _main.tex. See https://yihui.org/tinytex/r/#debugging for debugging tips.
����: Warning message:
In system2(..., stdout = if (use_file_stdout()) f1 else FALSE, stderr = f2) :
  '"xelatex"' not found
We can install MiKTex，add it to path，then update。
6、Package fontspec Error: The font "Inconsolata" cannot be found.
! Sorry, but miktex-makemf did not succeed.
! The log file hopefully contains the information to get MiKTeX going again:
We can install Inconsolata and Andale Momo, then add it to C:\windows\Fonts
