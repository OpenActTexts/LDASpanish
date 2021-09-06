# LDASpanish

The online version is available at https://openacttexts.github.io/LDASpanish/


### DOWNLOAD AND EDIT A LOCAL COPY OF THE BOOK

1.  Optional - Get reasonably recent versions of R and Rstudio. Sometimes, there can be conflicts if you are running very old versions these products. (Probably best to do this step at a later stage in case you run into problems that you can't debug.)
2.  Optional - Update packages. We have discovered conflicts between some of the advanced graphics/RGL and javascript in chapter 3 with old versions of some packages. Surprisingly, the one exception is the package bookdown. We found that an old version (0.21) works best. So, use this code:
    *  require(devtools)
    *  install_version("bookdown", version = "0.21", repos = "http://cran.us.r-project.org")
3.  Download a copy of the book. Go to Github, https://github.com/OpenActTextDev/LifeCon, hit the green "Code" button, download a .zip file and uncompress it.
4.  Open R-studio, go to "File==>Open Project". From the folder you just downloaded and uncompressed, select "LifeCon.Rproj".
5.  In R studio, open the file "PackagesLifeCon.Rmd" (but do not knit it). These are the packages that will be called when you compile the book, so install them now if needed.
6.  In R-studio, go to the upper right tab, hit "Build". This brings up a "Build Book" tab. Click the down arrow to the right and select "bookdown::gitbook". This starts the compile process.
7.  Upon successful compile, you should see a preview of the book. If it gets lost, go to the "docs" subfolder and open "index.html" in a browser, hopefully you see the compiled book.
8.  As you edit the book, go to the file "_bookdown.yml". This allows you to select the .Rmd files (and the order) that you wish to appear in the book.