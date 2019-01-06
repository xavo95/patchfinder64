# patchfinder64

Based of xerub's patchfinder64, adds various patches which should work across a variety of versions.

## Testing

This fork includes a testing portion, allowing us to confirm that the results returned from the patchfinder are valid.

To run the tests, you must do the following:
1. Run `./fetch_kernelcaches`, or run `python ./fetch_kernelcaches`. Please note this will download 8 iOS versions, and extract and decompress the kernelcaches. You can change which versions of iOS are to be downloaded in the file.
2. Run `make patchfinder64`
3. Make sure you have `nm` installed (its usually default on a variety of OSes)
4. Run `python test_versions.py`
