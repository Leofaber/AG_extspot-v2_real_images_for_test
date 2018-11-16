# AG_extspot-v2_real_images_for_test

## Model
Classes frequencies:
* bgFrequency(0.5)
* fluxFrequency(0.5)

Attributes mean and variance:
* bgAreaDistribution( 259.313, 114.337 )
* bgPhotonsInBlob( 2.70782, 1.06004 )
* bgPhotonsCloseness( 2.8795, 1.41748 )
* fluxAreaDistribution( 240.756, 66.9674 )
* fluxPhotonsInBlob( 4.26807, 1.97511 )
* fluxPhotonsCloseness( 1.7331, 0.873429 )

## Test set
* RealImages/080514B.cts
* RealImages/090401B.cts
* RealImages/090510.cts
* RealImages/090510x.cts
* RealImages/100724B.cts

## Classification Logs
log080514B_080514B.txt
* 1 SOURCE 55 -33 98.3846 2008-05-14T09:57:02 1.37844e+08 50 080514B -1
* 2 BG 65 -14 14.153 2008-05-14T09:57:02 1.37844e+08 50 080514B -1

log090401B_090401B.txt
* 1 BG 216 -2 5.38874e-06 2009-04-01T08:36:30 1.6566e+08 50 090401B -1

log090510_090510.txt
* 1 SOURCE 29 -48 71.1078 2009-05-10T00:24:06 1.69e+08 50 090510 -1

log090510x_090510x.txt
* 1 SOURCE 34 -50 84.5987 2009-05-10T00:24:06 1.69e+08 50 090510x -1

log100724B_100724B.txt
* 1 SOURCE 134 33 100 2010-07-24T00:43:11 2.07017e+08 50 100724B -1

## Ran with
* module load agile-B25-r5
* export PFILES=/home/student/AG_extspot-v2/conf
* make clean
* make agextspot
* ./bin/AG_extspot-v2 log100724B.txt 7.5 MAPS/RealImages/100724B.cts 50 no None
* ./bin/AG_extspot-v2 log090510x.txt 7.5 MAPS/RealImages/090510x.cts 50 no None
* ./bin/AG_extspot-v2 log090510.txt 7.5 MAPS/RealImages/090510.cts 50 no None
* ./bin/AG_extspot-v2 log090401B.txt 7.5 MAPS/RealImages/090401B.cts 50 no None
* ./bin/AG_extspot-v2 log080514B.txt 7.5 MAPS/RealImages/080514B.cts 50 no None
