# Notes

## Build Spec

`.build_spec/` contains a representation of the expected contents of the `build/` directory after running `gradelw build`.

The identified `build/` directory requirements for **DOF Alpha** are

1. The `build/` directory shall contain `component.yaml`, the human readable unified yaml file of the entire **DOF Alpha** project
2. The `build/` directory shall contain `package/` directory containing all elements to be published to npm repo
  1. The `build/package/` directory shall contain `component.min.json`, the minified json representation of the unified yaml file of the enture **DOF Alpha** project.
  2. The `build/package/` directory shall contain a copy of the project's `package.json` file.
  3. The `build/package/` directory shall contain `build/package/docs/` directory containing Markdown and PDF copies of all generated documents
  4. The `build/package/` directory shall contain a copy of the project's `README.md` file.
  5. The `build/package/` directory shall contain a copy of the project's `LICENSE` file.