## Dotscience Pipeline example


```
ds project create pipeline-test
```

To run the pipeline:

```
ds run -v -p pipeline-test --upload-path . python test.py
```

This will upload, run test.py and then run additional pipeline steps (prints task ID into the file).