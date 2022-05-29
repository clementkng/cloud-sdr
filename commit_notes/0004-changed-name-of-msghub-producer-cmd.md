### Patch oddness:
None, the patch applies cleanly.

### Tests (but don't try to hard given these are old commits):
We might not be able to test commits in general because of the lack of keys.

### Other observations:
* Renames the msghub-pubsync to msghub-producer
* Adds info for how to run the msghub-consumer
* Adds a sync flag for producer, by default false, that if set to false allows the producer to send messages later (rather than synchronously sending a specified message or default message)
