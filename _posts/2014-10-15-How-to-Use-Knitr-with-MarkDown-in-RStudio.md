---
layout: post
---

###Why Knitr?


Knitr allows you to weave R code, results, and figures directly into a report. Knitr allows you to easily show your R code directly alongside the resulting output.

Time to get started....

1. Open RStudio and install the Knitr Package
  
   1. Click on the **Install** button in the packages tab as shown below
![alt text](http://frcamacho.github.io/images/install_R_package.png)

  2. Once you have clicked on the Install button, the following window should appear ![alt text](http://frcamacho.github.io/images/pop-up-window-install.png)
  
  3. Type **knitr** within the Packages text box and click install ![alt text](http://frcamacho.github.io/images/knitr-install.png)

2. Now, open a MarkDown file in RStudio File-> New File-> R Markdown![alt text](http://frcamacho.github.io/images/Add-MarkDown-file.png)

  1. The pop-up window shown below should appear as soon as you click on R MarkDown ![alt text](http://frcamacho.github.io/images/Mark-down-title.png)
Replace **"Untitled"** with whatever title you want your report to have. It will be the first text in your super nice lookin' report. For now, leave the **Default Output Format** as **HTML**. Don't worry you can switch your Output to either Word or PDF at anytime.

  2. You can go ahead and run this sample MarkDown file to produce a knit HTML output by clicking **Knit HTML**. ![alt text](http://frcamacho.github.io/images/knitpdf.jpg)

  3. If all is good then you should produce a knit HTML output as shown below:  ![alt text](http://frcamacho.github.io/images/markdown-output.png)
  


Now to explain more about syntax in MarkDown to produce the beautiful Knitr HTML document!

Basic Markdown Syntax 
--------------
 
 
 In Markdown, R code can be used to render R output or to simply display your R code for illustration like this: 


~~~
```{r}
 
# PLACE R CODE HERE 

```
~~~

You can also embed plots to your report in Markdown like this: 

    ```{r, echo=FALSE}
    plot(variable)
    ```

"echo" is a parameter in Markdown

    ```

    `echo = FALSE` # prevent printing of the R code that generated the plot.
    `echo = TRUE` # prints R code and the output of that R code 

    ```


For more stylistic functions in Markdown visit: 

https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet



#PDFs with Markdown and Knitr 


In MarkDown to **Knit PDFs** you will need to install **TeX**.

**Windows** require **MiKTeX**

[Download](http://miktex.org/download)

**Mac OS X** require **MacTex 2013+**

[Download](http://www.tug.org/mactex/index.html)

**Linux** require **TeX Live 2013+**

[Download](https://www.tug.org/texlive/quickinstall.html)


###Once TeX is installed on your computer knitting a PDF is easy! 



Change the **output** from *"HTML_document"* to *"pdf_document"* (Red Box in the image below) 

Finally click Knit PDF (in red)  CONGRATULATIONS you have successfully knitted a knitr PDF with Markdown in Rstudio! 

![alt text](http://frcamacho.github.io/images/final_knit.png)



