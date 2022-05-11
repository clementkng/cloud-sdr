### Patch oddness:
None, the patch applies cleanly.

### Tests (but don't try to hard given these are old commits):
Again, hard given the same difficulties in the last commit.

### Other observations:
* New msghub-consumer to consume the messages
* Split out many things from `msghub-pubsync.go` into a `util.go` file, such as printing output and other functions specific to publishing and consuming messages (which is used by both the publisher and consumer)
	* Add some new functions to further split out concerns: `SendSyncMessages`, `PopulateConfig`, `ConsumePartition`
* Add sarama-cluster- cluster extensions (now deprecated)
	* Partitions are used by the cluster to figure out where traffic is going
* Removed server keys/certs and added them to the .gitignore
* Removed confluent example
* Some additional changes ie a make clean target
	* `pubasync` was added to the .gitignore, but it doesn't seem to exist for now
