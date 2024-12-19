# new_local_repository BUILD overwrite bug

## Bazel 7.4.1 and 8.0.0

fails:
```sh
bazelisk build //:file
```
passes:
```sh
bazelisk build //:contents
```

## Bazel 6.5.0

passes:
```sh
bazelisk build //:file
```
```sh
bazelisk build //:contents
```
