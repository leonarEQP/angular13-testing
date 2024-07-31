# Angular 13 Testing

1. Create angular project 13.2.0 version<br>
   `npx -p @angular/cli@13.2.0 ng new angular-testing`

2. Remove jasmine and karma dependencies<br>
   `npm remove @types/jasmine jasmine-core karma karma-chrome-launcher karma-coverage karma-jasmine karma-jasmine-html-reporte`

3. Remove node_modules and package-lock.json for a clean installation ( optional)<br>
   `mkdir /s /q node_modules` and `del package-lock.json`

4. Install dependencies<br>

   `npm install`

5. Install jest<br>

   `npm install --save-dev jest@27.5.1 jest-preset-angular@11.1.1 @types/jest@27.4.1`

6. Create setup-jest.ts file and import jest preset angular<br>

   `echo > setup-jest.ts`
