# Friedman

# 1. Load devtools
library(devtools)

# 2. Create your package
create("C:/Users/yamsi/Documents/Friedman")

# 3. Set working directory
setwd("C:/Users/yamsi/Documents/Friedman")

# 4. Create DESCRIPTION file content
desc_text <- "Package: Friedman
Title: Tools for Visualizing and Evaluating Predictive Models
Version: 0.0.0.9000
Authors@R: person('Yesenia', 'Reinoso', email = 'yesenia.reinoso@example.com', role = c('aut','cre'))
Description: The Friedman package provides functions to visualize, evaluate, and compare predictive models using ggplot2 and dplyr.
Depends: R (>= 3.1.2)
Imports: ggplot2, dplyr, tidyr
License: CC0
LazyData: true
URL: https://github.com/yesireinos/Friedman
BugReports: https://github.com/yesireinos/Friedman/issues"

# 5. Write the DESCRIPTION file
writeLines(desc_text, "DESCRIPTION")

# 6. Check and build
devtools::check(".")
devtools::build(".")
