---
title       : Use Slidify/knitr/shiny
subtitle    : Get with the times Prasad!
author      : John Muschelli
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}l
widgets   : mathjax        # {io2012, html5slides, shower, dzslides, ...}l
mode        : selfcontained # {standalone, draft}
---

## Why use RStudio, I like my stuff!

[http://www.rstudio.com/ide/download/](http://www.rstudio.com/ide/download/)
* It's good, has a more polished IDE
* Works well while knitting (sans yarn)
* Highlighting/<span class="black"><b>autocomplete</b></span> in the editor
* Can still use the R.app IDE when doing most things

---

## Why use knitr - I document!

* Takes little (no) steps 
* `install.packages("knitr")`
* It's hip - you're young
* It's broader than LaTeX
* Has caching - run only parts of reports!
  * Sometimes stuff takes forever

---



# Why Slidify, I love (Powerpoint/Beamer/Google Docs/Prezi)

* Prezi is great when not going too crazy
  * Most times they make me dizzy
* Beamer is reproducible and still the standard for straight math
* Html has really cool things you can add on (but have to learn), but you can do it with the `mathjax` widget

$$
\beta_1 + \beta_2 = Slidify
$$

---


## Why html?
You can also add really cool things (think apps):

<object data="knitted_webGL.html" width="800" height="600"> <embed src="knitted_webGL.html" width="800" height="600"> </embed> Error: Embedded data could not be displayed. </object>

---

## Get Slidify

You can install Slidify, write a three page slide deck and publish it to Github, all in less than 5 minutes!

Step | Description      | Code
-----|------------------|------------------------------------------------------
0    | Install          | `require(devtools)`
     |                  | `install_github("slidify", "ramnathv")`
     |                  | `install_github("slidifyLibraries", "ramnathv")`
1    | Load             | `library(slidify)`
1    | Author           | `author("mydeck")`
2    | Edit             | Write in RMarkdown, separating slides with a blank line followed by three dashes `---`.
3    | Slidify          | `slidify("index.Rmd")`
4    | Publish          | `publish(user = "USER", repo = "REPO")`

---

## But I want to shine!

* First off- what is shiny
* `install.packages("shiny")`
* (Example)
* Make your `ui.R` and `server.R` and then run `runApp()` to start the server

---

## Pause

* If your mind is not blown, you should be done your pizza
  * You can leave now - I have nothing cooler to offer you
  * FYI - you're not really allowed to leave
  * Just kidding
  * Not really

---

## Example I've used for Shiny

* Had large longitudinal data - wanted to window it interactively
* SVG is not supported in standard Shiny (think lattice plots) - look up shiny sandbox
* RGL is starting to work with it ( but still clunky )

---

