# DashboardNg

### 1. Generate Project

To create a new project:
`ng new --no-standalone`

### 2. Skip test file generation

The project is configured to skip the generation of `.spec.ts` test files for various Angular schematics. This is done to streamline the development process by avoiding the creation of unnecessary test files.

In the `angular.json` file, the following configurations are added under the `schematics` section:

```json
"schematics": {
  "@schematics/angular:component": {
    "standalone": false,
    "skipTests": true
  },
  "@schematics/angular:class": {
    "skipTests": true
  },
  "@schematics/angular:directive": {
    "standalone": false,
    "skipTests": true
  },
  "@schematics/angular:guard": {
    "skipTests": true
  },
  "@schematics/angular:interceptor": {
    "skipTests": true
  },
  "@schematics/angular:pipe": {
    "standalone": false,
    "skipTests": true
  },
  "@schematics/angular:resolver": {
    "skipTests": true
  },
  "@schematics/angular:service": {
    "skipTests": true
  }
}
```
