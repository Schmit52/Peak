# Peak
\name{perfectPeakpackage-package}
\alias{perfectPeakpackage-package}
\alias{perfectPeakpackage}
\docType{package}
\title{
perfectPeak is a package that combines all with all
Finding perfect peaks
}
\description{
The perfectPeakpackage is how to calculate a value of autonomy for any mountain. This means more ore less a ranking of perfect peaks. The aim is to find THE perfect peak out of many peaks in the alps. Therefor a dominance, prominence and independence value calculation is necessary.
}
\details{
\tabular{ll}{
Package: \tab perfectPeakpackage\cr
Type: \tab Package\cr
Version: \tab 1.0\cr
Date: \tab 2015-01-31\cr
License: \tab GPL (>= 2)\cr
}
You can use the functions as it is or adapt it to your needs.
}
\author{
Theresa Schmitt

Maintainer: Schmit52@students.uni-marburg.de
Theresa Schmitt
}
\references{
Rauch. C. (2012): Der perfekte Gipfel.  Panorama, 2/2012, S. 112.
Leonhard, W. (2012): Eigenstaendigkeit von Gipfeln. -
}

\keyword{ package }
\seealso{
\code{\link{initEnvironGIS}},
\code{\link{calculateDominance}}, 
\code{\link{calculateProminence}}, \code{\link{calculateEvalue}}, 
\code{\link{makePeak}},
}
\examples{
if (run.makePeak) {
  final.peak.list<-makePeak(dem.in, peak.list,make.peak.mode,epsg.code, kernel.size)
} else {
  if (file.exists(peak.list)){
    final.peak.list<-read.table(peak.list, header = TRUE, sep = " ",dec='.')
  } else{
    stop('There is no valid peaklist')
  }
}
}
