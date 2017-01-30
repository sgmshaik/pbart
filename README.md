# pbart
Parallel implementation of Bayesian Additive Regression Trees using Apache Spark.

Original source code is from the following paper: 
**Particle Gibbs for Bayesian Additive Regression Trees**.  <br />
For instructions how to use the code see https://github.com/balajiln/pgbart

The modified version contains a few additional runtime parameters.  

--partitions ( Sets number of partititions for parallel processing )  <br />
--p_fvp ( 0: Disable  1: Enable ) Predictors are parallelized  <br />
--p_upv ( 0: Disable 	1: Enable ) Training ids are parallelized  <br />

New option to load data was also added:

--dataset data   <br />
--data_path=/.../dataset <br />

which loads the following files <br />
/.../dataset.train.x  <br />
/.../dataset.train.y  <br />
/.../dataset.test.x   <br />
/.../dataset.test.y  <br />
