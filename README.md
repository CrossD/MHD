1. Issue the following commands to install the re-requisite package:

devtools::install_github('CrossD/RFPCA')

2. Install MHD (metric halfspace depth):

install.packages('MHD_0.0.0.9000.tar.gz')

3. Feel free to check out the documentation and examples of MHD::MHD. Below is an additional example. 


library(MHD)
mfd <- manifold::createM('Sphere')

n <- 100
d <- 2
data <- t(manifold::rmfd(mfd, n, dimIntrinsic=d))

depthObj <- MHD(mfd, data) 


