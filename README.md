# oligo_melt_analyzer

I. Files
Readme.md
Oligo_melt_temp.Rmd

II. Description
An R Shiny program rendered in a web browser that analyzes absorbance vs. temperature data from an oligonucleotide melting spectrometer and determines melting temperature(s) (Tm) and baseline-adjusted hyperchromicity. Plots of Absorbance vs. temperature and dAbs/dtemp are generated in the browser and may be exported as a pdf file.  

II. Imports
The data are imported as csv files with columns of temp (column A) and absorbance (column B). The headers are temp and abs, respectively. See example file provided. 

III. User inputs and work flow
In tab 1, the user selects a file for analysis and enters a file name. The plot of absorbance vs. temp appears in the tab. The temperature range of the plot may then be adjusted by values in the entry boxes. 

Tab 2 displays the derivative plot.

In tab 3, the user enters a number of temperatures that are required for calculating Tm and hyperchromicity. These include temperature ranges on the baseline preceding and following the melt transition, which are used in correcting the baseline. 

Tab 4 displays results. A download button can be added to display the results tab in another browser tab which can then be printed as a pdf file. 