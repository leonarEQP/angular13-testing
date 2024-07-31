# Angular 13 Testing

1. Create angular project 13.2.0 version

   ```
   npx -p @angular/cli@13.2.0 ng new angular-testing
   ```

2. Remove jasmine and karma dependencies

   ```
   npm remove @types/jasmine jasmine-core karma karma-chrome-launcher karma-coverage karma-jasmine karma-jasmine-html-reporte
   ```

3. Remove node_modules and package-lock.json for a clean installation ( optional)

   ```
   mkdir /s /q node_modules` and `del package-lock.json
   ```

4. Install dependencies

   ```
   npm install
   ```

5. Install jest

   ```
   npm install --save-dev jest@27.5.1 jest-preset-angular@11.1.1 @types/jest@27.4.1
   ```

6. Create setup-jest.ts file and import jest preset angular

   ```
   echo > setup-jest.ts
   ```

   ```setup-jest.ts
   import 'jest-preset-angular/setup-jest';
   ```

7. Add jest config to package.json

   ```package.json
   "jest": {
   "preset": "jest-preset-angular",
   "setupFilesAfterEnv": [
    "<rootDir>/setup-jest.ts"
   ],
   "globalSetup": "jest-preset-angular/global-setup"
   }

   ```

8. Add jest config to tsconfig and tsconfig.spec

   ```tsconfig.json
   "types": [
   "jest"
   ]
   ```
