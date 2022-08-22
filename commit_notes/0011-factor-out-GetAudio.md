### Patch oddness:
None, the patch applies cleanly.

### Tests (but don't try to hard given these are old commits):
We might not be able to test commits in general because of the lack of keys.

### Other observations:
* Factors our getAudio (and other functions/structs that will now be sourced from `rtlsdr`)
	* `getAudio` function and `PowerDist` struct were defined in multiple places, so this DRYs up the code as well
* Some functional changes as well ie `label.main.go` doesn't rely on `getPower` anymore 	