### Patch oddness:
None, the patch applies cleanly.

### Tests (but don't try to hard given these are old commits):
Again, hard given the same difficulties in the last commit.

### Other observations:
* Confluent kafka version gets renamed and doesn’t work with IBM Message Hub.
* Configures verbosity setting and usage information.
* Allows for `go build` to be used, with a Makefile and gitignoring go executables.
* Introduces Verbose method that adds newlines for separate messages and splits out stderr messages from stdout.
* Allows a custom message to be sent (rather than “message 0” to “message 9”).
