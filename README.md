README
The tidy data set makes use of the data sets that have been provided by:
==================================================================
Human Activity Recognition Using Smartphones Dataset
Version 1.0
==================================================================
Jorge L. Reyes-Ortiz, Davide Anguita, Alessandro Ghio, Luca Oneto.
Smartlab - Non Linear Complex Systems Laboratory
DITEN - Università degli Studi di Genova.
Via Opera Pia 11A, I-16145, Genoa, Italy.
activityrecognition@smartlab.ws
www.smartlab.ws
==================================================================
The tidy data set contains: 180 records with 69 variables

These variables identify the unique subject/activity pair the variables relate to:

Subject: the integer subject ID. 30 Objects participated on the experiment
Activity Label: Factor with 6 different activities

	Walking
	Walking Upstairs
	Walking Downstairs
	Sitting
	Standing
	Laying

Activity: integer id of Activities.

All 66 other variables are the mean of a measurement per activity per Subject. This is indicated by the initial Mean of in the variable name. All values are numeric.

The other 66 variables are described below:
There are a few different kind of measurements on 3 axial levels.

The features selected for this database come from the accelerometer and gyroscope 3-axial raw signals tAcc-XYZ and tGyro-XYZ. 
These time domain signals indicated by 'Time' in the variable name were captured at a constant rate of 50 Hz. 
Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise.
Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) 
using another low pass Butterworth filter with a corner frequency of 0.3 Hz. 

Subsequently, the body linear acceleration and angular velocity were derived in time to obtain Jerk signals 
(MeanoftimeBodyAccelerometerJerk-XYZ and MeanoftimeBodyGyroscopeJerk-XYZ) and of these the mean was calculated per object and per activity.
Also the mean per subject per activity of the magnitude of these three-dimensional signals were calculated using the Euclidean 
norm (MeanoftimeBodyAccelerometerMagnitude, MeanoftimetGravityAccelerometerMagnitude, MeanoftimeBodyAccelerometerJerkMagnitude, 
MeanoftimeBodyGyroscopeMagnitude, MeanoftimeBodyGyroscopeJerkMagnitude). 

Finally the mean per subject per activity of a Fast Fourier Transform (FFT) was applied to some of these signals producing 
MeanoffrequencyBodyAccelerometer-XYZ, MeanoffrequencyBodyAccelerometerJerk-XYZ, MeanoffrequencyBodyGyroscope-XYZ, 
MeanoffrequencyBodyAccelerometerJerkMagnitude, MeanoffrequencyBodyGyroscopeMagnitude, MeanoffrequencyBodyGyroscopeJerkMagnitude. 

In some case the names of the Body vraiables in the original data was named BodyBody. That has changed to Body.


 $ MEANoftimeBodyAccelerometermean()-X                             : num  0.277 0.255 0.289 0.261 0.279 ...
 $ MEANoftimeBodyAccelerometermean()-Y                             : num  -0.01738 -0.02395 -0.00992 -0.00131 -0.01614 ...
 $ MEANoftimeBodyAccelerometermean()-Z                             : num  -0.1111 -0.0973 -0.1076 -0.1045 -0.1106 ...
 $ MEANoftimeBodyAccelerometerStandaardeviation()-X                : num  -0.284 -0.355 0.03 -0.977 -0.996 ...
 $ MEANoftimeBodyAccelerometerStandaardeviation()-Y                : num  0.11446 -0.00232 -0.03194 -0.92262 -0.97319 ...
 $ MEANoftimeBodyAccelerometerStandaardeviation()-Z                : num  -0.26 -0.0195 -0.2304 -0.9396 -0.9798 ...
 $ MEANoftimeGravityAccelerometermean()-X                          : num  0.935 0.893 0.932 0.832 0.943 ...
 $ MEANoftimeGravityAccelerometermean()-Y                          : num  -0.282 -0.362 -0.267 0.204 -0.273 ...
 $ MEANoftimeGravityAccelerometermean()-Z                          : num  -0.0681 -0.0754 -0.0621 0.332 0.0135 ...
 $ MEANoftimeGravityAccelerometerStandaardeviation()-X             : num  -0.977 -0.956 -0.951 -0.968 -0.994 ...
 $ MEANoftimeGravityAccelerometerStandaardeviation()-Y             : num  -0.971 -0.953 -0.937 -0.936 -0.981 ...
 $ MEANoftimeGravityAccelerometerStandaardeviation()-Z             : num  -0.948 -0.912 -0.896 -0.949 -0.976 ...
 $ MEANoftimeBodyAccelerometerJerkmean()-X                         : num  0.074 0.1014 0.0542 0.0775 0.0754 ...
 $ MEANoftimeBodyAccelerometerJerkmean()-Y                         : num  0.028272 0.019486 0.02965 -0.000619 0.007976 ...
 $ MEANoftimeBodyAccelerometerJerkmean()-Z                         : num  -0.00417 -0.04556 -0.01097 -0.00337 -0.00369 ...
 $ MEANoftimeBodyAccelerometerJerkStandaardeviation()-X            : num  -0.1136 -0.4468 -0.0123 -0.9864 -0.9946 ...
 $ MEANoftimeBodyAccelerometerJerkStandaardeviation()-Y            : num  0.067 -0.378 -0.102 -0.981 -0.986 ...
 $ MEANoftimeBodyAccelerometerJerkStandaardeviation()-Z            : num  -0.503 -0.707 -0.346 -0.988 -0.992 ...
 $ MEANoftimeBodyGyroscopemean()-X                                 : num  -0.0418 0.0505 -0.0351 -0.0454 -0.024 ...
 $ MEANoftimeBodyGyroscopemean()-Y                                 : num  -0.0695 -0.1662 -0.0909 -0.0919 -0.0594 ...
 $ MEANoftimeBodyGyroscopemean()-Z                                 : num  0.0849 0.0584 0.0901 0.0629 0.0748 ...
 $ MEANoftimeBodyGyroscopeStandaardeviation()-X                    : num  -0.474 -0.545 -0.458 -0.977 -0.987 ...
 $ MEANoftimeBodyGyroscopeStandaardeviation()-Y                    : num  -0.05461 0.00411 -0.12635 -0.96647 -0.98773 ...
 $ MEANoftimeBodyGyroscopeStandaardeviation()-Z                    : num  -0.344 -0.507 -0.125 -0.941 -0.981 ...
 $ MEANoftimeBodyGyroscopeJerkmean()-X                             : num  -0.09 -0.1222 -0.074 -0.0937 -0.0996 ...
 $ MEANoftimeBodyGyroscopeJerkmean()-Y                             : num  -0.0398 -0.0421 -0.044 -0.0402 -0.0441 ...
 $ MEANoftimeBodyGyroscopeJerkmean()-Z                             : num  -0.0461 -0.0407 -0.027 -0.0467 -0.049 ...
 $ MEANoftimeBodyGyroscopeJerkStandaardeviation()-X                : num  -0.207 -0.615 -0.487 -0.992 -0.993 ...
 $ MEANoftimeBodyGyroscopeJerkStandaardeviation()-Y                : num  -0.304 -0.602 -0.239 -0.99 -0.995 ...
 $ MEANoftimeBodyGyroscopeJerkStandaardeviation()-Z                : num  -0.404 -0.606 -0.269 -0.988 -0.992 ...
 $ MEANoftimeBodyAccelerometerMagnitudemean()                      : num  -0.137 -0.1299 0.0272 -0.9485 -0.9843 ...
 $ MEANoftimeBodyAccelerometerMagnitudeStandaardeviation()         : num  -0.2197 -0.325 0.0199 -0.9271 -0.9819 ...
 $ MEANoftimeGravityAccelerometerMagnitudemean()                   : num  -0.137 -0.1299 0.0272 -0.9485 -0.9843 ...
 $ MEANoftimeGravityAccelerometerMagnitudeStandaardeviation()      : num  -0.2197 -0.325 0.0199 -0.9271 -0.9819 ...
 $ MEANoftimeBodyAccelerometerJerkMagnitudemean()                  : num  -0.1414 -0.4665 -0.0894 -0.9874 -0.9924 ...
 $ MEANoftimeBodyAccelerometerJerkMagnitudeStandaardeviation()     : num  -0.0745 -0.479 -0.0258 -0.9841 -0.9931 ...
 $ MEANoftimeBodyGyroscopeMagnitudemean()                          : num  -0.161 -0.1267 -0.0757 -0.9309 -0.9765 ...
 $ MEANoftimeBodyGyroscopeMagnitudeStandaardeviation()             : num  -0.187 -0.149 -0.226 -0.935 -0.979 ...
 $ MEANoftimeBodyGyroscopeJerkMagnitudemean()                      : num  -0.299 -0.595 -0.295 -0.992 -0.995 ...
 $ MEANoftimeBodyGyroscopeJerkMagnitudeStandaardeviation()         : num  -0.325 -0.649 -0.307 -0.988 -0.995 ...
 $ MEANoffrequencyBodyAccelerometermean()-X                        : num  -0.2028 -0.4043 0.0382 -0.9796 -0.9952 ...
 $ MEANoffrequencyBodyAccelerometermean()-Y                        : num  0.08971 -0.19098 0.00155 -0.94408 -0.97707 ...
 $ MEANoffrequencyBodyAccelerometermean()-Z                        : num  -0.332 -0.433 -0.226 -0.959 -0.985 ...
 $ MEANoffrequencyBodyAccelerometerStandaardeviation()-X           : num  -0.3191 -0.3374 0.0243 -0.9764 -0.996 ...
 $ MEANoffrequencyBodyAccelerometerStandaardeviation()-Y           : num  0.056 0.0218 -0.113 -0.9173 -0.9723 ...
 $ MEANoffrequencyBodyAccelerometerStandaardeviation()-Z           : num  -0.28 0.086 -0.298 -0.934 -0.978 ...
 $ MEANoffrequencyBodyAccelerometerJerkmean()-X                    : num  -0.1705 -0.4799 -0.0277 -0.9866 -0.9946 ...
 $ MEANoffrequencyBodyAccelerometerJerkmean()-Y                    : num  -0.0352 -0.4134 -0.1287 -0.9816 -0.9854 ...
 $ MEANoffrequencyBodyAccelerometerJerkmean()-Z                    : num  -0.469 -0.685 -0.288 -0.986 -0.991 ...
 $ MEANoffrequencyBodyAccelerometerJerkStandaardeviation()-X       : num  -0.1336 -0.4619 -0.0863 -0.9875 -0.9951 ...
 $ MEANoffrequencyBodyAccelerometerJerkStandaardeviation()-Y       : num  0.107 -0.382 -0.135 -0.983 -0.987 ...
 $ MEANoffrequencyBodyAccelerometerJerkStandaardeviation()-Z       : num  -0.535 -0.726 -0.402 -0.988 -0.992 ...
 $ MEANoffrequencyBodyGyroscopemean()-X                            : num  -0.339 -0.493 -0.352 -0.976 -0.986 ...
 $ MEANoffrequencyBodyGyroscopemean()-Y                            : num  -0.1031 -0.3195 -0.0557 -0.9758 -0.989 ...
 $ MEANoffrequencyBodyGyroscopemean()-Z                            : num  -0.2559 -0.4536 -0.0319 -0.9513 -0.9808 ...
 $ MEANoffrequencyBodyGyroscopeStandaardeviation()-X               : num  -0.517 -0.566 -0.495 -0.978 -0.987 ...
 $ MEANoffrequencyBodyGyroscopeStandaardeviation()-Y               : num  -0.0335 0.1515 -0.1814 -0.9623 -0.9871 ...
 $ MEANoffrequencyBodyGyroscopeStandaardeviation()-Z               : num  -0.437 -0.572 -0.238 -0.944 -0.982 ...
 $ MEANoffrequencyBodyAccelerometerMagnitudemean()                 : num  -0.1286 -0.3524 0.0966 -0.9478 -0.9854 ...
 $ MEANoffrequencyBodyAccelerometerMagnitudeStandaardeviation()    : num  -0.398 -0.416 -0.187 -0.928 -0.982 ...
 $ MEANoffrequencyBodyAccelerometerJerkMagnitudemean()             : num  -0.0571 -0.4427 0.0262 -0.9853 -0.9925 ...
 $ MEANoffrequencyBodyAccelerometerJerkMagnitudeStandaardeviation(): num  -0.103 -0.533 -0.104 -0.982 -0.993 ...
 $ MEANoffrequencyBodyGyroscopeMagnitudemean()                     : num  -0.199 -0.326 -0.186 -0.958 -0.985 ...
 $ MEANoffrequencyBodyGyroscopeMagnitudeStandaardeviation()        : num  -0.321 -0.183 -0.398 -0.932 -0.978 ...
 $ MEANoffrequencyBodyGyroscopeJerkMagnitudemean()                 : num  -0.319 -0.635 -0.282 -0.99 -0.995 ...
 $ MEANoffrequencyBodyGyroscopeJerkMagnitudeStandaardeviation()    : num  -0.382 -0.694 -0.392 -0.987 -0.995 ...



License:
========
Use of this dataset in publications must be acknowledged by referencing the following publication [1] 

[1] Davide Anguita, Alessandro Ghio, Luca Oneto, Xavier Parra and Jorge L. Reyes-Ortiz. Human Activity Recognition on Smartphones using a Multiclass Hardware-Friendly Support Vector Machine. International Workshop of Ambient Assisted Living (IWAAL 2012). Vitoria-Gasteiz, Spain. Dec 2012

This dataset is distributed AS-IS and no responsibility implied or explicit can be addressed to the authors or their institutions for its use or misuse. Any commercial use is prohibited.

Jorge L. Reyes-Ortiz, Alessandro Ghio, Luca Oneto, Davide Anguita. November 2012.


> summary(Tidy_data)
    Subject                Activity_label    Activity   MEANoftimeBodyAccelerometermean()-X
 Min.   : 1.0   LAYING            :30     Min.   :1.0   Min.   :0.2216                     
 1st Qu.: 8.0   SITTING           :30     1st Qu.:2.0   1st Qu.:0.2712                     
 Median :15.5   STANDING          :30     Median :3.5   Median :0.2770                     
 Mean   :15.5   WALKING           :30     Mean   :3.5   Mean   :0.2743                     
 3rd Qu.:23.0   WALKING_DOWNSTAIRS:30     3rd Qu.:5.0   3rd Qu.:0.2800                     
 Max.   :30.0   WALKING_UPSTAIRS  :30     Max.   :6.0   Max.   :0.3015                     
 MEANoftimeBodyAccelerometermean()-Y MEANoftimeBodyAccelerometermean()-Z MEANoftimeBodyAccelerometerStandaardeviation()-X
 Min.   :-0.040514                   Min.   :-0.15251                    Min.   :-0.9961                                 
 1st Qu.:-0.020022                   1st Qu.:-0.11207                    1st Qu.:-0.9799                                 
 Median :-0.017262                   Median :-0.10819                    Median :-0.7526                                 
 Mean   :-0.017876                   Mean   :-0.10916                    Mean   :-0.5577                                 
 3rd Qu.:-0.014936                   3rd Qu.:-0.10443                    3rd Qu.:-0.1984                                 
 Max.   :-0.001308                   Max.   :-0.07538                    Max.   : 0.6269                                 
 MEANoftimeBodyAccelerometerStandaardeviation()-Y MEANoftimeBodyAccelerometerStandaardeviation()-Z
 Min.   :-0.99024                                 Min.   :-0.9877                                 
 1st Qu.:-0.94205                                 1st Qu.:-0.9498                                 
 Median :-0.50897                                 Median :-0.6518                                 
 Mean   :-0.46046                                 Mean   :-0.5756                                 
 3rd Qu.:-0.03077                                 3rd Qu.:-0.2306                                 
 Max.   : 0.61694                                 Max.   : 0.6090                                 
 MEANoftimeGravityAccelerometermean()-X MEANoftimeGravityAccelerometermean()-Y MEANoftimeGravityAccelerometermean()-Z
 Min.   :-0.6800                        Min.   :-0.47989                       Min.   :-0.49509                      
 1st Qu.: 0.8376                        1st Qu.:-0.23319                       1st Qu.:-0.11726                      
 Median : 0.9208                        Median :-0.12782                       Median : 0.02384                      
 Mean   : 0.6975                        Mean   :-0.01621                       Mean   : 0.07413                      
 3rd Qu.: 0.9425                        3rd Qu.: 0.08773                       3rd Qu.: 0.14946                      
 Max.   : 0.9745                        Max.   : 0.95659                       Max.   : 0.95787                      
 MEANoftimeGravityAccelerometerStandaardeviation()-X MEANoftimeGravityAccelerometerStandaardeviation()-Y
 Min.   :-0.9968                                     Min.   :-0.9942                                    
 1st Qu.:-0.9825                                     1st Qu.:-0.9711                                    
 Median :-0.9695                                     Median :-0.9590                                    
 Mean   :-0.9638                                     Mean   :-0.9524                                    
 3rd Qu.:-0.9509                                     3rd Qu.:-0.9370                                    
 Max.   :-0.8296                                     Max.   :-0.6436                                    
 MEANoftimeGravityAccelerometerStandaardeviation()-Z MEANoftimeBodyAccelerometerJerkmean()-X
 Min.   :-0.9910                                     Min.   :0.04269                        
 1st Qu.:-0.9605                                     1st Qu.:0.07396                        
 Median :-0.9450                                     Median :0.07640                        
 Mean   :-0.9364                                     Mean   :0.07947                        
 3rd Qu.:-0.9180                                     3rd Qu.:0.08330                        
 Max.   :-0.6102                                     Max.   :0.13019                        
 MEANoftimeBodyAccelerometerJerkmean()-Y MEANoftimeBodyAccelerometerJerkmean()-Z
 Min.   :-0.0386872                      Min.   :-0.067458                      
 1st Qu.: 0.0004664                      1st Qu.:-0.010601                      
 Median : 0.0094698                      Median :-0.003861                      
 Mean   : 0.0075652                      Mean   :-0.004953                      
 3rd Qu.: 0.0134008                      3rd Qu.: 0.001958                      
 Max.   : 0.0568186                      Max.   : 0.038053                      
 MEANoftimeBodyAccelerometerJerkStandaardeviation()-X MEANoftimeBodyAccelerometerJerkStandaardeviation()-Y
 Min.   :-0.9946                                      Min.   :-0.9895                                     
 1st Qu.:-0.9832                                      1st Qu.:-0.9724                                     
 Median :-0.8104                                      Median :-0.7756                                     
 Mean   :-0.5949                                      Mean   :-0.5654                                     
 3rd Qu.:-0.2233                                      3rd Qu.:-0.1483                                     
 Max.   : 0.5443                                      Max.   : 0.3553                                     
 MEANoftimeBodyAccelerometerJerkStandaardeviation()-Z MEANoftimeBodyGyroscopemean()-X MEANoftimeBodyGyroscopemean()-Y
 Min.   :-0.99329                                     Min.   :-0.20578                Min.   :-0.20421               
 1st Qu.:-0.98266                                     1st Qu.:-0.04712                1st Qu.:-0.08955               
 Median :-0.88366                                     Median :-0.02871                Median :-0.07318               
 Mean   :-0.73596                                     Mean   :-0.03244                Mean   :-0.07426               
 3rd Qu.:-0.51212                                     3rd Qu.:-0.01676                3rd Qu.:-0.06113               
 Max.   : 0.03102                                     Max.   : 0.19270                Max.   : 0.02747               
 MEANoftimeBodyGyroscopemean()-Z MEANoftimeBodyGyroscopeStandaardeviation()-X MEANoftimeBodyGyroscopeStandaardeviation()-Y
 Min.   :-0.07245                Min.   :-0.9943                              Min.   :-0.9942                             
 1st Qu.: 0.07475                1st Qu.:-0.9735                              1st Qu.:-0.9629                             
 Median : 0.08512                Median :-0.7890                              Median :-0.8017                             
 Mean   : 0.08744                Mean   :-0.6916                              Mean   :-0.6533                             
 3rd Qu.: 0.10177                3rd Qu.:-0.4414                              3rd Qu.:-0.4196                             
 Max.   : 0.17910                Max.   : 0.2677                              Max.   : 0.4765                             
 MEANoftimeBodyGyroscopeStandaardeviation()-Z MEANoftimeBodyGyroscopeJerkmean()-X MEANoftimeBodyGyroscopeJerkmean()-Y
 Min.   :-0.9855                              Min.   :-0.15721                    Min.   :-0.07681                   
 1st Qu.:-0.9609                              1st Qu.:-0.10322                    1st Qu.:-0.04552                   
 Median :-0.8010                              Median :-0.09868                    Median :-0.04112                   
 Mean   :-0.6164                              Mean   :-0.09606                    Mean   :-0.04269                   
 3rd Qu.:-0.3106                              3rd Qu.:-0.09110                    3rd Qu.:-0.03842                   
 Max.   : 0.5649                              Max.   :-0.02209                    Max.   :-0.01320                   
 MEANoftimeBodyGyroscopeJerkmean()-Z MEANoftimeBodyGyroscopeJerkStandaardeviation()-X
 Min.   :-0.092500                   Min.   :-0.9965                                 
 1st Qu.:-0.061725                   1st Qu.:-0.9800                                 
 Median :-0.053430                   Median :-0.8396                                 
 Mean   :-0.054802                   Mean   :-0.7036                                 
 3rd Qu.:-0.048985                   3rd Qu.:-0.4629                                 
 Max.   :-0.006941                   Max.   : 0.1791                                 
 MEANoftimeBodyGyroscopeJerkStandaardeviation()-Y MEANoftimeBodyGyroscopeJerkStandaardeviation()-Z
 Min.   :-0.9971                                  Min.   :-0.9954                                 
 1st Qu.:-0.9832                                  1st Qu.:-0.9848                                 
 Median :-0.8942                                  Median :-0.8610                                 
 Mean   :-0.7636                                  Mean   :-0.7096                                 
 3rd Qu.:-0.5861                                  3rd Qu.:-0.4741                                 
 Max.   : 0.2959                                  Max.   : 0.1932                                 
 MEANoftimeBodyAccelerometerMagnitudemean() MEANoftimeBodyAccelerometerMagnitudeStandaardeviation()
 Min.   :-0.9865                            Min.   :-0.9865                                        
 1st Qu.:-0.9573                            1st Qu.:-0.9430                                        
 Median :-0.4829                            Median :-0.6074                                        
 Mean   :-0.4973                            Mean   :-0.5439                                        
 3rd Qu.:-0.0919                            3rd Qu.:-0.2090                                        
 Max.   : 0.6446                            Max.   : 0.4284                                        
 MEANoftimeGravityAccelerometerMagnitudemean() MEANoftimeGravityAccelerometerMagnitudeStandaardeviation()
 Min.   :-0.9865                               Min.   :-0.9865                                           
 1st Qu.:-0.9573                               1st Qu.:-0.9430                                           
 Median :-0.4829                               Median :-0.6074                                           
 Mean   :-0.4973                               Mean   :-0.5439                                           
 3rd Qu.:-0.0919                               3rd Qu.:-0.2090                                           
 Max.   : 0.6446                               Max.   : 0.4284                                           
 MEANoftimeBodyAccelerometerJerkMagnitudemean() MEANoftimeBodyAccelerometerJerkMagnitudeStandaardeviation()
 Min.   :-0.9928                                Min.   :-0.9946                                            
 1st Qu.:-0.9807                                1st Qu.:-0.9765                                            
 Median :-0.8168                                Median :-0.8014                                            
 Mean   :-0.6079                                Mean   :-0.5842                                            
 3rd Qu.:-0.2456                                3rd Qu.:-0.2173                                            
 Max.   : 0.4345                                Max.   : 0.4506                                            
 MEANoftimeBodyGyroscopeMagnitudemean() MEANoftimeBodyGyroscopeMagnitudeStandaardeviation()
 Min.   :-0.9807                        Min.   :-0.9814                                    
 1st Qu.:-0.9461                        1st Qu.:-0.9476                                    
 Median :-0.6551                        Median :-0.7420                                    
 Mean   :-0.5652                        Mean   :-0.6304                                    
 3rd Qu.:-0.2159                        3rd Qu.:-0.3602                                    
 Max.   : 0.4180                        Max.   : 0.3000                                    
 MEANoftimeBodyGyroscopeJerkMagnitudemean() MEANoftimeBodyGyroscopeJerkMagnitudeStandaardeviation()
 Min.   :-0.99732                           Min.   :-0.9977                                        
 1st Qu.:-0.98515                           1st Qu.:-0.9805                                        
 Median :-0.86479                           Median :-0.8809                                        
 Mean   :-0.73637                           Mean   :-0.7550                                        
 3rd Qu.:-0.51186                           3rd Qu.:-0.5767                                        
 Max.   : 0.08758                           Max.   : 0.2502                                        
 MEANoffrequencyBodyAccelerometermean()-X MEANoffrequencyBodyAccelerometermean()-Y MEANoffrequencyBodyAccelerometermean()-Z
 Min.   :-0.9952                          Min.   :-0.98903                         Min.   :-0.9895                         
 1st Qu.:-0.9787                          1st Qu.:-0.95361                         1st Qu.:-0.9619                         
 Median :-0.7691                          Median :-0.59498                         Median :-0.7236                         
 Mean   :-0.5758                          Mean   :-0.48873                         Mean   :-0.6297                         
 3rd Qu.:-0.2174                          3rd Qu.:-0.06341                         3rd Qu.:-0.3183                         
 Max.   : 0.5370                          Max.   : 0.52419                         Max.   : 0.2807                         
 MEANoffrequencyBodyAccelerometerStandaardeviation()-X MEANoffrequencyBodyAccelerometerStandaardeviation()-Y
 Min.   :-0.9966                                       Min.   :-0.99068                                     
 1st Qu.:-0.9820                                       1st Qu.:-0.94042                                     
 Median :-0.7470                                       Median :-0.51338                                     
 Mean   :-0.5522                                       Mean   :-0.48148                                     
 3rd Qu.:-0.1966                                       3rd Qu.:-0.07913                                     
 Max.   : 0.6585                                       Max.   : 0.56019                                     
 MEANoffrequencyBodyAccelerometerStandaardeviation()-Z MEANoffrequencyBodyAccelerometerJerkmean()-X
 Min.   :-0.9872                                       Min.   :-0.9946                             
 1st Qu.:-0.9459                                       1st Qu.:-0.9828                             
 Median :-0.6441                                       Median :-0.8126                             
 Mean   :-0.5824                                       Mean   :-0.6139                             
 3rd Qu.:-0.2655                                       3rd Qu.:-0.2820                             
 Max.   : 0.6871                                       Max.   : 0.4743                             
 MEANoffrequencyBodyAccelerometerJerkmean()-Y MEANoffrequencyBodyAccelerometerJerkmean()-Z
 Min.   :-0.9894                              Min.   :-0.9920                             
 1st Qu.:-0.9725                              1st Qu.:-0.9796                             
 Median :-0.7817                              Median :-0.8707                             
 Mean   :-0.5882                              Mean   :-0.7144                             
 3rd Qu.:-0.1963                              3rd Qu.:-0.4697                             
 Max.   : 0.2767                              Max.   : 0.1578                             
 MEANoffrequencyBodyAccelerometerJerkStandaardeviation()-X MEANoffrequencyBodyAccelerometerJerkStandaardeviation()-Y
 Min.   :-0.9951                                           Min.   :-0.9905                                          
 1st Qu.:-0.9847                                           1st Qu.:-0.9737                                          
 Median :-0.8254                                           Median :-0.7852                                          
 Mean   :-0.6121                                           Mean   :-0.5707                                          
 3rd Qu.:-0.2475                                           3rd Qu.:-0.1685                                          
 Max.   : 0.4768                                           Max.   : 0.3498                                          
 MEANoffrequencyBodyAccelerometerJerkStandaardeviation()-Z MEANoffrequencyBodyGyroscopemean()-X
 Min.   :-0.993108                                         Min.   :-0.9931                     
 1st Qu.:-0.983747                                         1st Qu.:-0.9697                     
 Median :-0.895121                                         Median :-0.7300                     
 Mean   :-0.756489                                         Mean   :-0.6367                     
 3rd Qu.:-0.543787                                         3rd Qu.:-0.3387                     
 Max.   :-0.006236                                         Max.   : 0.4750                     
 MEANoffrequencyBodyGyroscopemean()-Y MEANoffrequencyBodyGyroscopemean()-Z
 Min.   :-0.9940                      Min.   :-0.9860                     
 1st Qu.:-0.9700                      1st Qu.:-0.9624                     
 Median :-0.8141                      Median :-0.7909                     
 Mean   :-0.6767                      Mean   :-0.6044                     
 3rd Qu.:-0.4458                      3rd Qu.:-0.2635                     
 Max.   : 0.3288                      Max.   : 0.4924                     
 MEANoffrequencyBodyGyroscopeStandaardeviation()-X MEANoffrequencyBodyGyroscopeStandaardeviation()-Y
 Min.   :-0.9947                                   Min.   :-0.9944                                  
 1st Qu.:-0.9750                                   1st Qu.:-0.9602                                  
 Median :-0.8086                                   Median :-0.7964                                  
 Mean   :-0.7110                                   Mean   :-0.6454                                  
 3rd Qu.:-0.4813                                   3rd Qu.:-0.4154                                  
 Max.   : 0.1966                                   Max.   : 0.6462                                  
 MEANoffrequencyBodyGyroscopeStandaardeviation()-Z MEANoffrequencyBodyAccelerometerMagnitudemean()
 Min.   :-0.9867                                   Min.   :-0.9868                                
 1st Qu.:-0.9643                                   1st Qu.:-0.9560                                
 Median :-0.8224                                   Median :-0.6703                                
 Mean   :-0.6577                                   Mean   :-0.5365                                
 3rd Qu.:-0.3916                                   3rd Qu.:-0.1622                                
 Max.   : 0.5225                                   Max.   : 0.5866                                
 MEANoffrequencyBodyAccelerometerMagnitudeStandaardeviation() MEANoffrequencyBodyAccelerometerJerkMagnitudemean()
 Min.   :-0.9876                                              Min.   :-0.9940                                    
 1st Qu.:-0.9452                                              1st Qu.:-0.9770                                    
 Median :-0.6513                                              Median :-0.7940                                    
 Mean   :-0.6210                                              Mean   :-0.5756                                    
 3rd Qu.:-0.3654                                              3rd Qu.:-0.1872                                    
 Max.   : 0.1787                                              Max.   : 0.5384                                    
 MEANoffrequencyBodyAccelerometerJerkMagnitudeStandaardeviation() MEANoffrequencyBodyGyroscopeMagnitudemean()
 Min.   :-0.9944                                                  Min.   :-0.9865                            
 1st Qu.:-0.9752                                                  1st Qu.:-0.9616                            
 Median :-0.8126                                                  Median :-0.7657                            
 Mean   :-0.5992                                                  Mean   :-0.6671                            
 3rd Qu.:-0.2668                                                  3rd Qu.:-0.4087                            
 Max.   : 0.3163                                                  Max.   : 0.2040                            
 MEANoffrequencyBodyGyroscopeMagnitudeStandaardeviation() MEANoffrequencyBodyGyroscopeJerkMagnitudemean()
 Min.   :-0.9815                                          Min.   :-0.9976                                
 1st Qu.:-0.9488                                          1st Qu.:-0.9813                                
 Median :-0.7727                                          Median :-0.8779                                
 Mean   :-0.6723                                          Mean   :-0.7564                                
 3rd Qu.:-0.4277                                          3rd Qu.:-0.5831                                
 Max.   : 0.2367                                          Max.   : 0.1466                                
 MEANoffrequencyBodyGyroscopeJerkMagnitudeStandaardeviation()
 Min.   :-0.9976                                             
 1st Qu.:-0.9802                                             
 Median :-0.8941                                             
 Mean   :-0.7715                                             
 3rd Qu.:-0.6081                                             
 Max.   : 0.2878     







