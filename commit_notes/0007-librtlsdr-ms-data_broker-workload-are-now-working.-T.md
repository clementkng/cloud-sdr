### Patch oddness:
None, the patch applies cleanly.

### Tests (but don't try to hard given these are old commits):
We might not be able to test commits in general because of the lack of keys. However, the changes to `cloud/sdr` in this commit are inherently tested by the other changes.

### Other observations:
* Adds new stt (speech to text) package that defines some utility functions for new edge sdr examples
	* Adds a wav header
	* Transcribes audio by sending it to IBM Watson
* This stt package was added here, but technically not part of `cloud/sdr`. I believe at some point later it will be moved to `sdr2evtstreams`
* A period in the commit message truncates the file name
* Other changes covered in less detail because technically outside `cloud/sdr`
	* data_broker for passing along and processing data
	* librtlsdr for defining software defined radio that can be queried for audio and power
	* random_model for training, but this is broken	
