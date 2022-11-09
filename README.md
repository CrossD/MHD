1. Issue the following commands to install the re-requisite package:

`install.packages("manifold")`

2. Install MHD (metric halfspace depth):

`devtools::install_github("CrossD/MHD")`

3. Documentation and examples are available under `MHD::MHD`. Below is an additional example. 

```
library(MHD)
mfd <- manifold::createM('Sphere')

n <- 100
d <- 2
data <- t(manifold::rmfd(mfd, n, dimIntrinsic=d))

depthObj <- MHD(mfd, data) 
```

