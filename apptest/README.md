# Continuous Integration - Jenkins and Co  

Cette application doit être buildée avec Node.

Avant chaque étape: npm install
Les étapes:
* _Build_: `npm run build-ci`  
* _Test_: `npm run test-ci`
* _Test sans coverage_: `npm run test-ci-without-coverage` 
* _Sonar_: `sonar-scanner -Dsonar.projectKey=<projectKey> -Dsonar.organization=<organisation>`

## Exercice 1 - Build FreeStyle [Jenkins](http://localhost:8080)    
      
Configurer un build *Jenkins FreeStyle* pour:

* Builder et archiver les artifacts
* Tester avec et sans coverage, utiliser un paramètre booléen pour determiner quel test exécuter. 
  
## Exercice 2 - Build Pipeline [Jenkins](http://localhost:8080)

Ecrire un *Jenkinsfile* pour:

* Builder et archiver les artifacts
* Tester avec et sans coverage, utiliser un paramètre booléen pour determiner quel test exécuter et archiver le rapport de coverage si celui a été créé (./coverage/lcov-report)