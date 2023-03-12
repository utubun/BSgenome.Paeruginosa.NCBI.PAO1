
# BSgenome.Paeruginosa.NCBI.PAO1

<!-- badges: start -->
[![Lifecycle: experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://lifecycle.r-lib.org/articles/stages.html#experimental)
<!-- badges: end -->

The package provides a full genome assembly of P. aeruginosa str. PAO1. Data source: [NCBI](https://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/000/006/765/GCF_000006765.1_ASM676v1/).

## Installation

You can install the development version of BSgenome.Paeruginosa.NCBI.PAO1 from [GitHub](github.com) with:

``` r
devtools::install_github('utubun/BSgenome.Paeruginosa.NCBI.PAO1')
```

## Example

Load *P. aeruginosa* str. PAO1 genome, and assign it ot the variable `genome`:

``` r
library(BSgenome.Paeruginosa.NCBI.PAO1)

genome <- BSgenome.Paeruginosa.NCBI.PAO1
```

Get the information about the genome:

``` r
sprintf(
  'Genome:\t%s\nName:\t%s\nOrganism:\t%s\nProvider:\t%s\nReleased:\t%s',
  sapply(c(bsgenomeName, commonName, organism, provider, releaseDate), \(f) {f(genome)})
)
```

List the methods available for the given object class:

```r
methods(class = class(genome))
```

# More examples

``` r
help(package = 'BSgenome')
```
