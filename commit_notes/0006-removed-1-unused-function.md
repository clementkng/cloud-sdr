### Patch oddness:
None, the patch applies cleanly.

### Tests (but don't try to hard given these are old commits):
We might not be able to test commits in general because of the lack of keys.

### Other observations:
* Removed unused function Close from util since the producer and consumer have the responsibility of closing the client (and as of this commit no unique client objects are even created in the producer/consumer)
