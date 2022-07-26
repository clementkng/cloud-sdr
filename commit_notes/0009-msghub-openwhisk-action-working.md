### Patch oddness:
None, the patch applies cleanly.

### Tests (but don't try to hard given these are old commits):
We might not be able to test commits in general because of the lack of keys. Here, we can't additionally test because we don't have access to the target org and space (and the Hovitos objects within).

### Other observations:
* Openwhisk action now works to process SDR data from IBM message hub
* Followup from last commit
* Adds makefile that utilizes `bx wsk` CLI
	* Has some untested targets
	* `bx wsk` CLI binds serverless function to IBM cloud functions, in a scalable FAAS model
* Updates `msgreceive.js` to simply print out the value of messages passed to it
* Adds a test for `msgreceive.js`
