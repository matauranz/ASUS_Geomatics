RTKLIB

INTRODUCTION

RTKLIB is a simple and portable C-library for constructing RTK-GPS (Realtime
Kinematic GPS) positioning applications. RTKLIB includes

- matirx and vector functions
- time and string functions
- coordinates transformation
- tropospheric and ionosphric models
- RINEX files reading function
- navigation algorithms
- OTF integer ambiguity resolution by LAMBDA/MLAMBDA
- single point positioning
- RTK-GPS relative positioning

RTKLIB also includes a post-mission baseline analysis application RNX2RTKP
using RTKLIB functions. RNX2RTKP inputs RINEX OBS/NAV files of rover and
reference station, and computes the rover positions and track by RTK-GPS
positioning with OTF integer ambiguity resolution.

RTKLIB can use BLAS/LAPACK or Intel MKL for matrix routines.

INSTALL, BUILD AND USE

Console applications were tested on gcc
GUI applications need borland turbo C++.

PACKAGE

rtklib_{ver}.zip

./src    source programs
./bin    application binary programs
./app    application source programs and make environments
  ./rnx2rtkp  rinex to rtk positioning
  ./pos2kml   convert position to google earth kml
  ./convbin   convert receiver log file to rinex
  ./sbspos    positioning with sbas corrections
  ./sbsdump   dump sbas messages
  ./rtkpost   gui post-positioning 
  ./rtkpost_mkl gui post-positioning with intel mkl
  ./rtkplot   gui plot solutions or observation data
  ./rtkconv   gui receiver log converter
  ./rtknavi   gui realtime rtk positioning
  ./strsvr    gui stream server
  ./str2str   command line stream server
  ./srctblbrows ntrip source table browser
  ./appcmn    common application routines
  ./icon      common application icons
./util   utilities
./test   test programs and data
./doc    documents
./mkl    intel mkl library include and lib for borland environment

LICENSE

RTKLIB is licensed under GPLv3. (http://gplv3.fsf.org/)

HISTORY

ver.1.0    2007/01/25 new release
ver.1.1    2007/03/20 add rnx2rtkp_gui, fix bugs, improve performance
ver.2.1.0  2008/07/15 refactored, add applications
ver.2.1.1  2008/10/19 fix bugs
ver.2.2.0  2009/01/20 add stream.c,rtksvr.c,preceph.c in src
                      add rtknavi,rtkpost_mkl,srctblbrows,strsvr,str2str

--------------------------------------------------------------------------------

           Copyright (C) 2007-2009 by T.TAKASU, All rights reserved.

