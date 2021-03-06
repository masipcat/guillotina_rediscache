2.1.1 (unreleased)
------------------

- Nothing changed yet.


2.1.0 (2018-11-20)
------------------

- Upgrade to Guillotina >= 4.3
  [bloodbare]

2.0.4 (2018-10-06)
------------------

- Do not fail memory cache if not configured
  [vangheem]


2.0.3 (2018-07-20)
------------------

- Remove old guillotina compatibility for py 3.7
  [bloodbare]


2.0.2 (2018-06-18)
------------------

- Improve size calculation
  [jordic]


2.0.1 (2018-06-15)
------------------

- Change default cache size to 209715200
  [vangheem]


2.0.0 (2018-06-15)
------------------

- Cache based on memory size instead of total number of keys
  [jordic]


1.3.4 (2018-04-03)
------------------

- Fix fixture
  [vangheem]


1.3.3 (2018-04-03)
------------------

- Upgrade testing for guillotina 3.0
  [vangheem]


1.3.2 (2018-03-26)
------------------

- Use after commit hook to update data for file manager implementation
  [vangheem]


1.3.1 (2018-03-19)
------------------

- Fix redis file manager finish method
  [vangheem]


1.3.0 (2018-03-19)
------------------

- Provide redis file manager
  [vangheem]


1.2.0 (2018-03-14)
------------------

- Upgrade to work with guillotina 2.4.x
  [vangheem]


1.1.6 (2018-03-01)
------------------

- Handle errors while canceling task init task
  [vangheem]


1.1.5 (2018-03-01)
------------------

- Handle errors while canceling task
  [vangheem]


1.1.4 (2018-02-15)
------------------

- Fix cache stats endpoint
  [vangheem]


1.1.3 (2018-01-22)
------------------

- Be able to disable deleting group of cache keys together with `cluster_mode`
  option.
  [vangheem]


1.1.2 (2018-01-17)
------------------

- Fix using redis.delete when keys are of length 0
  [vangheem]


1.1.1 (2018-01-17)
------------------

- batch all cache deletes into one request
  [vangheem]


1.1.0 (2018-01-12)
------------------

- Push cache updates to redis subscriber. This should improve cache hits dramatically
  [vangheem]


1.0.14 (2018-01-10)
-------------------

- Only run invalidation task if we have keys to invalidate
  [vangheem]


1.0.13 (2017-12-15)
-------------------

- Improve request performance
  [vangheem]

- Change the way we're using the redis pool so it reuses connections
  [vangheem]


1.0.12 (2017-11-30)
-------------------

- Missing await statement for `self.get_redis()`
  [vangheem]


1.0.11 (2017-11-08)
-------------------

- Handle CancelledError
  [vangheem]


1.0.10 (2017-11-06)
-------------------

- upgrade for guillotina 2.0.0
  [vangheem]


1.0.9 (2017-10-23)
------------------

- Fix handling connection objects and releasing back to pool
  [vangheem]


1.0.8 (2017-10-23)
------------------

- Fix use of pool
  [vangheem]

1.0.7 (2017-10-23)
------------------

- Use pickle instead of json from load/dumps because it is much faster
  [vangheem]


1.0.6 (2017-10-19)
------------------

- Use ujson
  [vangheem]


1.0.5 (2017-10-02)
------------------

- Track all keys needing invalidation and do invalidation in an async task
  so the request can finish faster.
  [vangheem]


1.0.4 (2017-05-29)
------------------

- Test fixes
  [vangheem]


1.0.3 (2017-05-26)
------------------

- Fix delete not properly invalidating cache
  [vangheem]


1.0.2 (2017-05-15)
------------------

- Fix channel publishing invalidations
  [vangheem]


1.0.1 (2017-05-15)
------------------

- Fix release


1.0.0 (2017-05-15)
------------------

- initial release
