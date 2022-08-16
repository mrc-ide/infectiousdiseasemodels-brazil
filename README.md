## Introduction to Mathematical Models of the Epidemiology & Control of Infectious Diseases

For more information, see [infectiousdiseasemodels.org](http://www.infectiousdiseasemodels.org/) or [to the applications](https://shiny.dide.imperial.ac.uk/infectiousdiseasemodels-2021)

## Running in local mode

Ensure that you have rtools installed [instructions for recent R are here](https://cran.r-project.org/bin/windows/Rtools/rtools42/rtools.html)

Download the 2019 library (set of packages). You can get this from https://mrcdata.dide.ic.ac.uk/shiny/lib-2019.zip - it's about 100MB. Unzip this in the root of this directory.

If you're lazy you can run:

```
options(timeout = 600)
download.file("https://mrcdata.dide.ic.ac.uk/shiny/lib-2019.zip", "lib-2019.zip", mode = "wb")
unzip("lib-2019.zip")
```

There are two Rstudio project files, one in `introduction`, the other in `flu`; open these in Rstudio.

You should see the console print something like:

```
Using library at '/home/rfitzjoh/Documents/Projects/shiny/infectiousdiseasemodels-brazil/lib-2019'
```

which indicates that it has found the correct library.

Then open the `run.R` file (it will be open next time you open the project). At the top right of the editor pane you should see a "**Run App**" button, click this to launch the app.

If you close the page and want to reopen it, fancy a different browser, or want to run a second session, paste the URL from the console into your browser. It will be something like `http://127.0.0.1:3404` though the last digits will change each time the application runs. You do not need to run the Rstudio project multiple times to open multiple copies.
