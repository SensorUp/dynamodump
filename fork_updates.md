# Fork Updates

Many forks have been created for this repository since the last time it was updated. This document attempts to identify the ones with the most useful changes.

* <https://github.com/10eTechnology/dynamodump/commit/568a29e26fc056a46e9babf1db118b417fe6251b>
  * adding multiprocessing support
* <https://github.com/batistan/dynamodump/commit/644a337cc6193ddb89747410123cf3c1b1adaacb>
  * Add default read and write capacity for all tables
    * If a table (or its indices) has autoscaling capacity, DynamoDB's describe-tables operation will report zero read and write capacity.  This works, until you have to restore the table, at which point it will complain that you can't specify zero as a read or write capacity for a table or index. This commit sets such capacities to a default of 25 units.
* <https://github.com/bchew/dynamodump/compare/master...bimp:master>
  * added the ability to restore a table with Time To Live (TTL) property
* <https://github.com/brendangibat/dynamodump/commit/42f15f168b872d24358dfe302cd82ac48593bbb0>
  * adds path to dump data
* <https://github.com/btrajkovski/dynamodump/commit/20c79d1f6f078012693474b34c7e132291c8fe9f>
  * handle not overwriting newer versions of records (needs to have version field)
* <https://github.com/callum-p/dynamodump/compare/master...mergermarket:master>
  * Seems to set ad hoc billing correctly
  * Needs boto3 - missing exceptions
* <https://github.com/cantenesse/dynamodump/commits/master>
  * adds s3 backup
* <https://github.com/christophgysin/dynamodump/commits/master>
  * fix provisioning GSI capacities
* <https://github.com/CliveJL/dynamodump/commit/faa6564900b8832d9bca1e6b0c111ff05420a913>
  * Update to Boto3 support. Add support for `PAY_PER_REQUEST` billing mode (On-demand).
* <https://github.com/bchew/dynamodump/compare/master...dannyn:master>
  * Filter attributes on backup
* <https://github.com/bchew/dynamodump/compare/master...dixahq:master>
  * Adds S3 upload
* <https://github.com/bchew/dynamodump/compare/master...EldarSagirov:master>
  * Adds security token for local DynamoDB
* <https://github.com/bchew/dynamodump/compare/master...faiyeah:master>
  * Fixed process hangs when backing up a non-exist table
* <https://github.com/bchew/dynamodump/compare/master...LimbicEntertainment:master>
  * FIxes On Demand - moves to Boto3
* <https://github.com/bchew/dynamodump/compare/master...rstaveley:master>
  * Fixes On Demand - moves to Boto3; adds support for ECS, Autoscaling and AWS batch
* <https://github.com/bchew/dynamodump/compare/master...taherbs:master>
  * Adding make automation + Dockerizing further
* <https://github.com/bchew/dynamodump/compare/master...uktrade:master>
  * Expand docker config (conflicts)
* <https://github.com/xebia-france/dynamodump>
  * This branch is 10 commits ahead, 1 commit behind bchew:master.
  * Implement read rate limiting
