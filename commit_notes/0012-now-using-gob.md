### Patch oddness:
None, the patch applies cleanly.

### Tests (but don't try to hard given these are old commits):
We might not be able to test commits in general because of the lack of keys.

### Other observations:
* Now the `data_broker` edge service is connecting to a msghub topic called "sdr-audio" and publishing good radio station audio there
* Not exactly sure what gob means
* I'm not sure how this touches `cloud/sdr`, these reverse merges are confusing me
