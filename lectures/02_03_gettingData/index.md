---
title       : Getting data
subtitle    : 
author      : Jeffrey Leek
job         : Johns Hopkins Bloomberg School of Public Health
logo        : bloomberg_shield.png
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow   # 
url:
  lib: ../../libraries
  assets: ../../assets
widgets     : [mathjax]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
---






## My belief about statisticians

* Define the question
* Define the ideal data set
* <redtext>Determine what data you can access </redtext>
* <redtext>Obtain the data </redtext>
* <redtext>Clean the data </redtext>
* Exploratory data analysis
* Statistical prediction/modeling
* Interpret results
* Challenge results
* Synthesize/write up results
* Create reproducible code


---


## Why? 

<center> "Real scientists make their own data" -Sean Taylor</center>

<center> "Real scientists make (and know how to get) their own data" -Jeff </center>

1. Most major contributions to real science involve data collection (by you/others)
2. Making/getting your own data gives you priveledged access to scientific findings
3. If you create the data you will understand it better
4. You can do things like experimental design (e.g. randomized experiments)

[http://seanjtaylor.com/post/41463778912/real-scientists-make-their-own-data](http://seanjtaylor.com/post/41463778912/real-scientists-make-their-own-data)


---

## What you wish data looked like

<img class=center src=../../assets/img/03_ObtainingData/excel.png height=450>


---

## What does data really look like? 

<img class=center src=../../assets/img/03_ObtainingData/fastq.png height=450/>


[http://brianknaus.com/software/srtoolbox/s_4_1_sequence80.txt](http://brianknaus.com/software/srtoolbox/s_4_1_sequence80.txt)


--- 

## What does data really look like? 

<img class=center src=../../assets/img/03_ObtainingData/twitter.png height= 450/>


[https://dev.twitter.com/docs/api/1/get/blocks/blocking](https://dev.twitter.com/docs/api/1/get/blocks/blocking)

---

## What does data really look like?


<img class=center src=../../assets/img/03_ObtainingData/medicalrecord.png height=400/>


[http://blue-button.github.com/challenge/](http://blue-button.github.com/challenge/)



---

## What does data really look like?

<img class=center src=../../assets/img/fmri.jpeg height= 450/>


[http://spectrum.ieee.org/tech-talk/biomedical/imaging/sorting-fmri-with-textmining-software](http://spectrum.ieee.org/tech-talk/biomedical/imaging/sorting-fmri-with-textmining-software)

---

## Where is data?


<img class=center src=../../assets/img/harddrive.jpg height= 450/>

[http://en.wikipedia.org/wiki/Sneakernet](http://en.wikipedia.org/wiki/Sneakernet)

[http://en.wikipedia.org/wiki/File:USB-Hard-Drive.jpg](http://en.wikipedia.org/wiki/File:USB-Hard-Drive.jpg)

---

## Where is data?

<img class=center src=../../assets/img/03_ObtainingData/databases.png height=400/>


[http://rickosborne.org/blog/2010/02/infographic-migrating-from-sql-to-mapreduce-with-mongodb/](http://rickosborne.org/blog/2010/02/infographic-migrating-from-sql-to-mapreduce-with-mongodb/)


---

## Where is data?

<img class=center src=../../assets/img/03_ObtainingData/twitter.png height= 450/>

[https://dev.twitter.com/docs/api/1/get/blocks/blocking](https://dev.twitter.com/docs/api/1/get/blocks/blocking)


---

## Where is data?

<img class=center src=../../assets/img/03_ObtainingData/baltimore.png height= 450/>

[https://data.baltimorecity.gov/](https://data.baltimorecity.gov/)

---

## Definition of data

<q>Data are values of qualitative or quantitative variables, belonging to a set of items.</q>

[http://en.wikipedia.org/wiki/Data](http://en.wikipedia.org/wiki/Data)

---

## Definition of data
<q>Data are values of qualitative or quantitative variables, belonging to a <redtext>set of items</redtext>.</q>

[http://en.wikipedia.org/wiki/Data](http://en.wikipedia.org/wiki/Data)

__Set of items__: Sometimes called the population; the set of objects you are interested in

---

## Definition of data
<q>Data are values of qualitative or quantitative <redtext>variables</redtext>, belonging to a set of items.</q>

[http://en.wikipedia.org/wiki/Data](http://en.wikipedia.org/wiki/Data)

__Variables__: A measurement or characteristic of an item.


---

## Definition of data
<q>Data are values of <redtext>qualitative</redtext> or <redtext>quantitative</redtext> variables, belonging to a set of items.</q>

[http://en.wikipedia.org/wiki/Data](http://en.wikipedia.org/wiki/Data)


__Qualitative__: Country of origin, sex, treatment

__Quantitative__: Height, weight, blood pressure

---

## Raw versus processed data

__Raw data__
* The original source of the data
* Often hard to use for data analyses
* Data analysis _includes_ processing
* Raw data may only need to be processed once

[http://en.wikipedia.org/wiki/Raw_data](http://en.wikipedia.org/wiki/Raw_data)

__Processed data__
* Data that is ready for analysis
* Processing can include merging, subsetting, transforming, etc.
* There may be standards for processing
* All steps should be recorded 

[http://en.wikipedia.org/wiki/Computer_data_processing](http://en.wikipedia.org/wiki/Computer_data_processing)

---

## An example of a processing pipeline

<img class=center src=../../assets/img/03_ObtainingData/hiseq.jpeg height=450/>

[http://www.illumina.com.cn/support/sequencing/sequencing_instruments/hiseq_1000.asp](http://www.illumina.com.cn/support/sequencing/sequencing_instruments/hiseq_1000.asp)

---

## An example of a processing pipeline

<img class=center src=../../assets/img/03_ObtainingData/processing.png height=400 />

[http://www.cbcb.umd.edu/~hcorrada/CMSC858B/lectures/lect22_seqIntro/seqIntro.pdf](http://www.cbcb.umd.edu/~hcorrada/CMSC858B/lectures/lect22_seqIntro/seqIntro.pdf)

---

---

## The raw data


* The strange binary file your measurement machine spits out
* The unformatted Excel file with 10 worksheets the company you contracted with sent you
* The complicated JSON data you got from scraping the Twitter API
* The hand-entered numbers you collected looking through a microscope

_You know the raw data is in the right format if you_ 

1. Ran no software on the data
2. Did not manipulate any of the numbers in the data
3. You did not remove any data from the data set
4. You did not summarize the data in any way

[https://github.com/jtleek/datasharing](https://github.com/jtleek/datasharing)


---

## The tidy data

1. Each variable you measure should be in one column
2. Each different observation of that variable should be in a different row
3. There should be one table for each "kind" of variable
4. If you have multiple tables, they should include a column in the table that allows them to be linked

_Some other important tips_

* Include a row at the top of each file with variable names. 
* Make variable names human readable AgeAtDiagnosis instead of AgeDx
* In general data should be saved in one file per table.

[https://github.com/jtleek/datasharing](https://github.com/jtleek/datasharing)


---

## The code book

1. Information about the variables (including units!) in the data set not contained in the tidy data
2. Information about the summary choices you made
3. Information about the experimental study design you used


_Some other important tips_

* A common format for this document is a Word/text file. 
* There should be a section called "Study design" that has a thorough description of how you collected the data. 
* There must be a section called "Code book" that describes each variable and its units.


[https://github.com/jtleek/datasharing](https://github.com/jtleek/datasharing)


---

## The instruction list 

* Ideally a computer script (in R :-), but I suppose Python is ok too...)
* The input for the script is the raw data
* The output is the processed, tidy data
* There are no parameters to the script

In some cases it will not be possible to script every step. In that case you should provide instructions like: 

1. Step 1 - take the raw file, run version 3.1.2 of summarize software with parameters a=1, b=2, c=3
2. Step 2 - run the software separately for each sample
3. Step 3 - take column three of outputfile.out for each sample and that is the corresponding row in the output data set

[https://github.com/jtleek/datasharing](https://github.com/jtleek/datasharing)



---

## Why is the instruction list important? 

<img class=center src=../../assets/img/03_ObtainingData/rr.png height=200 />

<img class=center src=../../assets/img/03_ObtainingData/rrcolbert.jpeg height=250>


[http://www.colbertnation.com/the-colbert-report-videos/425748/april-23-2013/austerity-s-spreadsheet-error](http://www.colbertnation.com/the-colbert-report-videos/425748/april-23-2013/austerity-s-spreadsheet-error)

---

## Get/set your working directory

* A basic component of working with data is knowing your working directory
* The two main commands are ```getwd()``` and ```setwd()```. 
* Be aware of relative versus absolute paths
  * __Relative__ - ```setwd("./data")```, ```setwd("../")```
  * __Absolute__ - ```setwd("/Users/jtleek/data/")```
* Important difference in Windows ```setwd("C:\\Users\\Andrew\\Downloads")```

---

## Checking for and creating directories

* ```file.exists("directoryName")``` will check to see if the directory exists
* ```dir.create("directoryName")``` will create a directory if it doesn't exist
* Here is an example checking for a "data" directory and creating it if it doesn't exist


```r
if(!file.exists("data")){
  dir.create("data")
}
```



---

## Getting data from the internet - download.file()

* Downloads a file from the internet
* Even if you could do this by hand, helps with reproducibility
* Important parameters are _url_, _destfile_, _method_
* Useful for downloading tab-delimited, csv, and other files


---

## Example - Baltimore camera data


<img class=center src=../../assets/img/03_ObtainingData/cameras.png height=500>

[https://data.baltimorecity.gov/Transportation/Baltimore-Fixed-Speed-Cameras/dz54-2aru](https://data.baltimorecity.gov/Transportation/Baltimore-Fixed-Speed-Cameras/dz54-2aru)


---

## Example - Baltimore camera data

<img class=center src=../../assets/img/03_ObtainingData/cameraslink.png height=500>

[https://data.baltimorecity.gov/Transportation/Baltimore-Fixed-Speed-Cameras/dz54-2aru](https://data.baltimorecity.gov/Transportation/Baltimore-Fixed-Speed-Cameras/dz54-2aru)


---

## Download a file from the web


```r
fileUrl <- "https://data.baltimorecity.gov/api/views/dz54-2aru/rows.csv?accessType=DOWNLOAD"
download.file(fileUrl,destfile="./data/cameras.csv",method="curl")
list.files("./data")
```

```
[1] "cameras.csv"  "cameras.xlsx" "movies.txt"  
```

```r
dateDownloaded <- date()
dateDownloaded
```

```
[1] "Thu Jan 30 10:25:10 2014"
```


---

## Some notes about download.file()

* If the url starts with _http_ you can use download.file()
* If the url starts with _https_ on Windows you may be ok
* If the url starts with _https_ on Mac you may need to set _method="curl"_
* If the file is big, this might take a while
* Be sure to record when you downloaded. 

---

## Loading flat files - read.table()

* This is the main function for reading data into R
* Flexible and robust but requires more parameters
* Reads the data into RAM - big data can cause problems
* Important parameters _file_, _header_, _sep_, _row.names_, _nrows_
* Related: _read.csv()_, _read.csv2()_


---


## Example: Baltimore camera data


```r
cameraData <- read.table("./data/cameras.csv",sep=",",header=TRUE)
head(cameraData)
```

```
                         address direction      street  crossStreet               intersection
1       S CATON AVE & BENSON AVE       N/B   Caton Ave   Benson Ave     Caton Ave & Benson Ave
2       S CATON AVE & BENSON AVE       S/B   Caton Ave   Benson Ave     Caton Ave & Benson Ave
3 WILKENS AVE & PINE HEIGHTS AVE       E/B Wilkens Ave Pine Heights Wilkens Ave & Pine Heights
4        THE ALAMEDA & E 33RD ST       S/B The Alameda      33rd St     The Alameda  & 33rd St
5        E 33RD ST & THE ALAMEDA       E/B      E 33rd  The Alameda      E 33rd  & The Alameda
6        ERDMAN AVE & N MACON ST       E/B      Erdman     Macon St         Erdman  & Macon St
                       Location.1
1 (39.2693779962, -76.6688185297)
2 (39.2693157898, -76.6689698176)
3  (39.2720252302, -76.676960806)
4 (39.3285013141, -76.5953545714)
5 (39.3283410623, -76.5953594625)
6 (39.3068045671, -76.5593167803)
```


---

## Example: Baltimore camera data

read.csv sets _sep=","_ and _header=TRUE_ 

```r
cameraData <- read.csv("./data/cameras.csv")
head(cameraData)
```

```
                         address direction      street  crossStreet               intersection
1       S CATON AVE & BENSON AVE       N/B   Caton Ave   Benson Ave     Caton Ave & Benson Ave
2       S CATON AVE & BENSON AVE       S/B   Caton Ave   Benson Ave     Caton Ave & Benson Ave
3 WILKENS AVE & PINE HEIGHTS AVE       E/B Wilkens Ave Pine Heights Wilkens Ave & Pine Heights
4        THE ALAMEDA & E 33RD ST       S/B The Alameda      33rd St     The Alameda  & 33rd St
5        E 33RD ST & THE ALAMEDA       E/B      E 33rd  The Alameda      E 33rd  & The Alameda
6        ERDMAN AVE & N MACON ST       E/B      Erdman     Macon St         Erdman  & Macon St
                       Location.1
1 (39.2693779962, -76.6688185297)
2 (39.2693157898, -76.6689698176)
3  (39.2720252302, -76.676960806)
4 (39.3285013141, -76.5953545714)
5 (39.3283410623, -76.5953594625)
6 (39.3068045671, -76.5593167803)
```



---

## Some more important parameters

* _quote_ - you can tell R whether there are any quoted values quote="" means no quotes.
* _na.strings_ - set the character that represents a missing value. 
* _nrows_ - how many rows to read of the file (e.g. nrows=10 reads 10 lines).
* _skip_ - number of lines to skip before starting to read

_In my experience, the biggest trouble with reading flat files are quotation marks ` or " placed in data values, setting quote="" often resolves these_.



---

## Example: Baltimore camera data

read.csv sets _sep=","_ and _header=TRUE_ 

```r
cameraData <- scan("./data/cameras.csv",sep=",",what="character")
str(cameraData)
```

```
 chr [1:486] "address" "direction" "street" "crossStreet" "intersection" ...
```

```r
cameraData <- matrix(cameraData,byrow=TRUE,ncol=6)
```





---

## Excel files

_Still probably the most widely used format for sharing data_

<img class=center src=../../assets/img/03_ObtainingData/excel2.png height=450>


[http://office.microsoft.com/en-us/excel/](http://office.microsoft.com/en-us/excel/)

---

## Download the file to load


```r
if(!file.exists("data")){dir.create("data")}
fileUrl <- "https://data.baltimorecity.gov/api/views/dz54-2aru/rows.xlsx?accessType=DOWNLOAD"
download.file(fileUrl,destfile="./data/cameras.xlsx",method="curl")
dateDownloaded <- date()
```


---

## read.xlsx(), read.xlsx2() {xlsx package}


```r
library(xlsx)
cameraData <- read.xlsx("./data/cameras.xlsx",sheetIndex=1,header=TRUE)
head(cameraData)
```

```
                         address direction      street  crossStreet               intersection
1       S CATON AVE & BENSON AVE       N/B   Caton Ave   Benson Ave     Caton Ave & Benson Ave
2       S CATON AVE & BENSON AVE       S/B   Caton Ave   Benson Ave     Caton Ave & Benson Ave
3 WILKENS AVE & PINE HEIGHTS AVE       E/B Wilkens Ave Pine Heights Wilkens Ave & Pine Heights
4        THE ALAMEDA & E 33RD ST       S/B The Alameda      33rd St     The Alameda  & 33rd St
5        E 33RD ST & THE ALAMEDA       E/B      E 33rd  The Alameda      E 33rd  & The Alameda
6        ERDMAN AVE & N MACON ST       E/B      Erdman     Macon St         Erdman  & Macon St
                       Location.1
1 (39.2693779962, -76.6688185297)
2 (39.2693157898, -76.6689698176)
3  (39.2720252302, -76.676960806)
4 (39.3285013141, -76.5953545714)
5 (39.3283410623, -76.5953594625)
6 (39.3068045671, -76.5593167803)
```



---

## Reading specific rows and columns


```r
colIndex <- 2:3
rowIndex <- 1:4
cameraDataSubset <- read.xlsx("./data/cameras.xlsx",sheetIndex=1,
                              colIndex=colIndex,rowIndex=rowIndex)
cameraDataSubset
```

```
  direction      street
1       N/B   Caton Ave
2       S/B   Caton Ave
3       E/B Wilkens Ave
```


---

## Further notes

* The _write.xlsx_ function will write out an Excel file with similar arguments.
* _read.xlsx2_ is much faster than _read.xlsx_ but for reading subsets of rows may be slightly unstable. 
* The [XLConnect](http://cran.r-project.org/web/packages/XLConnect/index.html) package has more options for writing and manipulating Excel files
* The [XLConnect vignette](http://cran.r-project.org/web/packages/XLConnect/vignettes/XLConnect.pdf) is a good place to start for that package
* In general it is advised to store your data in either a database
or in comma separated files (.csv) or tab separated files (.tab/.txt) as they are easier to distribute.