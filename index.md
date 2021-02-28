

Airlines (Stat2Data) dataset 
========================================================
author: Arturo Prieto Tirado
date: 29/01/2021
autosize: true
font-import: https://fonts.googleapis.com/css2?family=Akaya+Kanadaka&display=swap
font-family: 'Akaya Kanadaka' 

<style>
/* css for initial slide */
.section .reveal .state-background {
    background-image: url(https://www.ecestaticos.com/imagestatic/clipping/868/9ca/8689ca73237158da46e457a120354717/por-que-los-aviones-comerciales-no-llevan-paracaidas-para-casos-de-emergencia.jpg?mtime=1593793065);
    background-position: center center;
    background-attachment: fixed;
    background-repeat: no-repeat;
    background-size: 100% 100%;
}

/* css for the rest of slides */
body{

background-color: #cce6ff;
data-transition: "fade";

}
</style>


The dataset 
========================================================
incremental: true


Describes 10333 OnTime arrivals for American and Delta airlines at LaGuardia (New York) and O'Hare (Chicago) airports using 5 categorical variables:

- Airline : Either American or Delta
- Airport : Either LGA=La Guardia or ORD=O'Hare
- On time : Yes or no
- IndOHare: Is the airport ORD? (1=yes or 0=no)
- IndDelta: Is the airline Delta? (1=yes or 0=no)


Variable Distribution 
========================================================
transition: fade

<img src="index-figure/unnamed-chunk-1-1.png" title="plot of chunk unnamed-chunk-1" alt="plot of chunk unnamed-chunk-1" width="60%" />



Variable Distribution 2
========================================================
incremental:true
transition:fade
- 71 % of the flights belong to American Airlines and 29% to Delta.

- 45% of the flights arrived to La Guardia and 55% to Chicago O'Hare

- 80% of the flights arrived on time

- IndOHare and IndDelta contain the same information as airline and airport


Correlations
========================================================

Able to study if flights are delayed or not. See correlations with respect to OnTime.

![plot of chunk unnamed-chunk-2](index-figure/unnamed-chunk-2-1.png)

Conclusions
===============================================================
incremental:true

- Redundant variables like IndOHare and IndDelta are just 0/1 binary representations on the binary categorical variables airport and airline.

- Punctuality can be a variable of interest for study. However, there is low correlation and few variables, so it would be interesting to expand the dataset with many more variables and/or more important ones to build models.
