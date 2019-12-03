# Jenkinsfile
# Maven project Build and test.
#!/usr/bin/env groovy

node { git url: 'https://github.com/lounge76/WebDriverTest.git' def mvn = tool 'M3' sh "${mvn}/bin/mvn -B -Dmaven.test.failure.ignore verify" step([$class: 'JUnitResultArchiver', testResults: '**/target/foobar/TEST-*.xml']) }