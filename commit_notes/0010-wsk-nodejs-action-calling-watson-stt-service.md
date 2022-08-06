### Patch oddness:
None, the patch applies cleanly.

### Tests (but don't try to hard given these are old commits):
We might not be able to test commits in general because of the lack of keys.

### Other observations:
* The action now actually calls out to Watson STT (as opposed to just saying it does)
	* Some hardcoded logic ie Watson STT credentials
* Cleanup and enhancements
	* Add `.gitignore`
	* Adds docs for make targets and Node packages installed in the Openwhisk functions environment
	* Updates test to log response
