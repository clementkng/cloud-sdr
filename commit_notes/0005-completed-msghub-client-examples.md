### Patch oddness:
None, the patch applies cleanly.

### Tests (but don't try to hard given these are old commits):
We might not be able to test commits in general because of the lack of keys.

### Other observations:
* Mass rename of example-go-publisher directory to example-go-clients
* Adds documentation: 
	* How to use your own certificate
	* Links to docs for more unique go packages
* Moves `SendSyncMessage` and `SendSyncMessages`, from util into msghub-producer
* Moves  `ConsumePartition` from util into msghub-consumer
