### Patch oddness:
None, the patch applies cleanly.

### Tests (but don't try to hard given these are old commits):
We might not be able to test commits in general because of the lack of keys. However, this commit doesn't seem connected to anything else within `cloud/sdr`. As noted in the commit message, this function works but also errors somehow?

### Other observations:
* Adds new asynchronous function that prints out info about messages pertaining to cats and their colors
	* IBM Cloud function
	* Based on naming, probably evolved to this file, which is still in `cloud/sdr` as of the time of this commit: https://github.com/open-horizon/examples/blob/master/cloud/sdr/data-processing/ibm-functions/actions/msgreceive.js
