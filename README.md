# New Zealand Covid-19 Case Data

This data has been quickly pulled together by the _New Zealand Herald_ data journalism team - if you
have any issues please contact Chris Knox by email <chris.knox@nzherald.co.nz> or via
[Twitter](https://twitter.com/vizowl)

**Updated to 'As at 9.30 am, 26 March 2020'**

- Daily totals from Feb 28 - NA where data wasn't reported [csv](https://github.com/nzherald/nz-covid19-data/raw/master/data/days.csv) and [excel](https://github.com/nzherald/nz-covid19-data/raw/master/data/days.xlsx)
- DHB totals starting March 26 [csv](https://github.com/nzherald/nz-covid19-data/raw/master/data/dhb-cases.csv) and [excel](https://github.com/nzherald/nz-covid19-data/raw/master/data/dhb-cases.xlsx)



## March 26 update

The Ministry appears to no longer be reporting indivdual cases and has switched to a cases by DHB
based reporting.

Since the data released previously was not reported by DHB there is no way to link the two.
Therefore the final versions of the cases data are now in `data/archive` I have also copied the
could used to produce those files to `data/archive/archive.R`

Hopefully the Ministry continues to publish cases details and I will resurrect this code.

## A little detail

The data is from https://www.health.govt.nz/our-work/diseases-and-conditions/covid-19-novel-coronavirus/covid-19-current-cases

The data is downloaded and cleaned up using R - all code is in `_drake.R`

There are a selection of files in the `data` directory.

I am using drake to process manage the update process - I will turn this into an R data package when
I get the time.

Pull requests are very welcome.

The code is a MIT licensed and the data is under the Ministry of Health's creative commons license https://www.health.govt.nz/about-site/copyright
