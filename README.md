# AngularTesting

1. Create angular project 13.2.0 version
   `npx -p @angular/cli@13.2.0 ng new angular-testing`

2. Remove jasmine and karma dependencies
   `npm remove @types/jasmine jasmine-core karma karma-chrome-launcher karma-coverage karma-jasmine karma-jasmine-html-reporte`

3. Remove node_modules and package-lock.json for a clean installation ( optional)

`mkdir /s /q node_modules` and `del package-lock.json`
