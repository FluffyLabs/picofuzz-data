# picofuzz-data

Test data repository for the [typeberry-testing](https://github.com/fluffylabs/typeberry-testing) project.

## Purpose

There repo is designed to be imported as a Git submodule in the `fluffylabs/typeberry-testing` repository.
Contains `picofuzz-data` generated out of latest `jam-test-vectors`.

## Maintenance

The test data is automatically updated through GitHub Actions:

- **Daily Updates**: A scheduled workflow runs daily at 11:00 AM UTC
- **Update Process**:
  1. Updates the `jam-test-vectors` submodule to the latest version
  2. Regenerates picofuzz data using `populate.sh`
  3. Creates a pull request with the updated data

To manually regenerate the picofuzz data:

```bash
./populate.sh
```
