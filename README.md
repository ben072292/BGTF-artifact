This work is based on Apache Spark, please configure spark enviroment using appropriate Spark configuration files for your own settings. Note: please assign at least 32g memory for the driver and each executor by doing ```--driver-memory 32g``` and ```--executor-memory 32g```

To run statitical evaluation using BGTF (e.g, N subjects, N = 6 - 15, 9 risk patterns: 0.02, 1-mix, 2-mix, 3-mix, 4-mix, 0.05, 0.1, 0.15, 0.2, each with 4 test selection rules), Please launch POSET-COVID-19-0.0.1-SNAPSHOT.jar file through bgtf_start_simulation.sh following the example below:

```./bgtf_start_simulation.sh <Number of Subjects> <Risk Pattern> <Test Selection Rule>```

For ```<Risk Pattern>```

1 : 0.02

2 : 1-mix

3 : 2-mix

4 : 3-mix

5 : 4-mix

6 : 0.05

7 : 0.1

8 : 0.15

9 : 0.2

For ```<Test Selection Rule>```

1 : BGHA

2 : 2-BGHA

3 : 3-BGHA

4 : 4-BGHA

The simulation will generate a set of statistical and performance evaluation summary, named by ```<Number of Subjects>-<Risk-Pattern>-<Test Selection Rule>-<MM-DD-YYYY HH-MM-SS>.csv```, indicating which pool setting is used for the set of simulaitons with an attached time stamp.



To run performance evaluation using BGTF (e.g 12 subjects with 0.02, 1-mix and 0.2 risk patterns, each with 4 test selection rules using 4 implementation schemes). Please launch POSET-COVID-19-0.0.1-SNAPSHOT.jar file through bgtf_start_simulation.sh following the example below:

```./bgtf_start_simulation.sh <Number of Subjects>```


The simulation will generate a set of statistical and performance evaluation summary, named by ```<Number of Subjects>-<Risk-Pattern>-<MM-DD-YYYY HH-MM-SS>.csv```, indicating which pool setting is used for the set of simulaitons with an attached time stamp.
