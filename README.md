# How to handle scaling data across indexes

- Since the number of shards are static and decided when you create the index, what to do when your queries are not scaling?
- Most of the queries are temporal in nature, i.e. there is a timerange in the queries.
- The idea is to _**timeshard**_ the indexes.

## Approach 1 - On Application side
- Example: have an index for data spanning across May & June. On the application side, figure out the indexes 
- Create new indexes based on the size of index


## Approach 2 - On ES Side


Using index lifecycle management (ILM)
