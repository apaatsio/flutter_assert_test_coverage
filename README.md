# Flutter issue 22508

This is a minimal reproducible project to demonstrate the issue "Test coverage
shows only some asserts coveraged."

See https://github.com/flutter/flutter/issues/22508

## Instructions

```
flutter test --coverage
cat ./coverage/lcov.info
```

### Expected output
```
SF:lib/assert.dart
DA:1,1
DA:2,1
LF:2
LH:2
end_of_record
```

### Actual output

```
SF:lib/assert.dart
DA:1,1
DA:2,0
LF:2
LH:1
end_of_record
```
