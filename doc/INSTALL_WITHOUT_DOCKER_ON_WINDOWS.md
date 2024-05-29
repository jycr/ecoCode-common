In the case Docker / Docker Desktop cannot be used to develop and test a plugin (network issues, workstation issues, corporate policies...), the alternate option is to install and run Sonarqube locally  
---
# Prequisites 
 * required java version (c.f. starter pack)
 * Sonarqube install found here : https://www.sonarsource.com/products/sonarqube/downloads/

# Install Instructions
 * Download the latest Community edition of Sonarqube from https://www.sonarsource.com/products/sonarqube/downloads/
 * Unzip the file in a folder *X*
 * Define an environment variable called __SONARQUBE_INSTALL__ pointing to this *X* path

# Install a plugin 
 * Build the jar file of the plugin according to the instructions given in the README file of the project's plugin
 * Copy the produced jar file (*ecocode-<language>-plugin-X.Y.Z-SNAPSHOT.jar*) from the *target/* folder of the plugin (for maven-based plugins) into the  folder of the Sonarqube install
 * Start Sonarqube using the *StartSonar.bat* from the *bin\windows-x86-64* path
