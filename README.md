# Useful postgreSQL docker template

## Useful pages
* ### [pgAdmin Page](http://localhost:5050/browser/).
* ### [Postgres exporter Page](http://localhost:9187/metrics).
* ### [Dozzle Page](http://localhost:8080)


## Secrets settings


**Only for local development!** You should specify `secrets` for services in the secret folder.
**Please note that the secrets are stored as files.**

## For developers
### The following has been changed in the config file:

* shared_buffers: Increase the shared memory buffer to accommodate more data in memory.

* effective_cache_size: Increase the cache size to improve the planner's decisions.

* work_mem: Increase the working memory to allow for more complex query operations.

* maintenance_work_mem: Increase the maintenance memory to speed up vacuum and index creation operations.

* max_connections: Adjust the maximum allowed connections based on your application's needs.

* checkpoint_completion_target: Increase the checkpoint completion target to spread checkpoint I/O over a longer period.