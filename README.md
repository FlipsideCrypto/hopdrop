# Topic: HOP Airdrop

[HOP](https://hop.exchange/) is a bridge exchange across EVM blockchains and L2s like Ethereum, Optimism, and Polygon. They launched their HOP token to retroactive users and use it to boost rewards to liquidity providers on their bridge.

For a deeper dive into the context, you can check out the report on our [research site](https://science.flipsidecrypto.xyz/research/) at [hop-drop](https://science.flipsidecrypto.xyz/hopdrop/).

If you aren't interested in code and want the short summary of the drop, you can check out the email sized [hop-drop](https://flipsidecrypto.beehiiv.com/p/hop-drop) on our research beehiiv and subscribe to get (summaries of) the best crypto research direct to your inbox.

# Reproduce Analysis

All analysis is reproducible using the R programming language. You'll need (1) an shroomDK API key to copy our SQL queries and extract data from the [FlipsideCrypto data app](https://next.flipsidecrypto.xyz/); and (2) renv to get the exact package versions we used.

## shroomDK

shroomDK is an R package that accesses the FlipsideCrypto REST API; it is also available for Python. You pass SQL code as a string to our API and get up to 1M rows of data back!

Check out the [documentation](https://docs.flipsidecrypto.com/shroomdk-sdk/get-started) and get your free API Key today.

## renv

renv is a package manager for the R programming language. It ensures analysis is fully reproducible by tracking the exact package versions used in the analysis.

`install.packages('renv')`

## Instructions

To replicate this analysis please do the following:

1.  Clone this repo.
2.  Save your API key into a .txt file as 'api_key.txt' (this exact naming allows the provided .gitignore to ignore your key and keep it off github).
3.  Open the `hopdrop` R Project file in your R IDE (we recommend, RStudio).
4.  Confirm you have renv installed.
5.  Restore the R environment using `renv::restore()` while in the `hopdrop` R Project.
6.  You can now run `hopdrop.Rmd`

If any errors arise, double check you have saved your API key in the expected file name and format.
