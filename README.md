## Dotscience Pipeline example

Goals:
1. Trigger CircleCI workflows after Dotscience training tasks

## Setup

1. CircleCI part: https://circleci.com/docs/2.0/getting-started/#section=getting-started
2. Dotscience part:

  ```
  ds project create pipeline-test
  ```

  To run the pipeline:

  ```
  ds run -v -p pipeline-test --upload-path . python test.py
  ```

  This will upload, run test.py and then run additional pipeline steps (prints task ID into the file).

