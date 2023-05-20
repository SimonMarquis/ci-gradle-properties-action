# CI Gradle properties

Copy Gradle properties file to the CI's home directory.  
This is especially useful if you need to provide (or override) specific properties on top of the project's properties. 

## Usage

See [action.yml](https://github.com/SimonMarquis/ci-gradle-properties-action/blob/main/action.yml)

```yml
steps:
- uses: actions/checkout@v3
- uses: SimonMarquis/ci-gradle-properties-action@v1
  with:
    path: .github/gradle.properties
```

| Input  | Description |
|--------|-------------|
| `path` | Gradle properties file path. Default is `.github/gradle.properties`. |
