JHUGen
======
To install, run

$ lib/downloadcollier.sh

then

$ cd JHUGenerator/

$ make

then

$ ./JHUGen [arguments]

In case of error related to .dylib, run

$ install_name_tool -add_rpath ../lib/COLLIER  ./JHUGen

which may happen on the latest MacOS

Example ZH commands:

Process=50

$ ./JHUGen PDFSet=2 Collider=1 Process=50 DecayMode1=0 Unweighted=0 VegasNc1=100000 VegasNc2=100000 HbbDK=0 DataFile=data/qq_ZH_llH_50 FacScheme=2 RenScheme=2 MuFacMultiplier=1.0 MuRenMultiplier=1.0 ghz1=2.0,0.0

Process=51

./JHUGen PDFSet=2 Collider=1 Process=51 VH_PC=lo DecayMode1=0 Unweighted=0 VegasNc1=100000 VegasNc2=100000 HbbDK=0 DataFile=data/qq_ZH_llH_51 FacScheme=2 RenScheme=2 MuFacMultiplier=1.0 MuRenMultiplier=1.0 ghz1=2.0,0.0

add argument for writing out .LHE if needed.

