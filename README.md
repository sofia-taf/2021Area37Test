# area37

Experiment with Rishi, demonstrating how the SOFIA analysis for Area 37
(Mediterranean and Black Sea) can run in TAF.

## How to run

Install the TAF package from CRAN.

Then open R in the `area37` directory and run:

```
library(TAF)
taf.bootstrap()
sourceAll()
```

The `sourceAll` function runs the TAF scripts sequentially in alphabetical
order:

```
data.R
model.R
output.R
report.R
```

An alternative to `sourceAll` is the `makeAll` function, which omits TAF scripts
that have already been run.

See also:

[SOFIA-TAF tutorial](https://github.com/sofia-taf/doc/blob/main/taf_tutorial.md)
