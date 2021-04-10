To run simulations using BGTF with all pool settings used for evaluation, (e.g 12 subjects with 0.02, 1-mix and 0.2 risk patterns, each with 4 test selection rules using 4 implementation schemes). Please lunch bayesgrouptestbackend/target/POSET-COVID-19-0.0.1-SNAPSHOT.jar file through bgtf_start_simulation.sh following the example below:

```./bgtf_start_simulation.sh <Number of Subject>```


The simulation will generate a set of statistical and performance evaluation summary, named by ```<Number of Subjects>-<Risk-Pattern>-<MM-DD-YYYY HH-MM-SS>.csv```, indicating which pool setting is used for the set of simulaitons with an attached time stamp.

Note: Please configure your spark enviroment using the Spark configuration files for your own settings, please assign at least 32g memory for both driver and executors.
