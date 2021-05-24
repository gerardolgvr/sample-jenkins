properties([
  parameters([
       [$class: 'DynamicReferenceParameter',
     choiceType: 'ET_FORMATTED_HIDDEN_HTML',
     description: '',
     name: 'YOUR_PARAMETER_NAME',
     omitValueField: true,
     referencedParameters: '',
     script: [
         $class: 'GroovyScript',
         fallbackScript: [classpath: [], sandbox: false, script: ''],
             script: [
                 classpath: [], 
                 sandbox: false, 
                 script: 'return "<input type=\\"date\\" name=\\"value\\" value=\\"\\" />"'
             ]
         ]
     ]

 ])
])
pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo "hola"
      }
    }
    stage('Output Date') {
        steps {
            script {
                println params.YOUR_PARAMETER_NAME
            }
        }
    }
  }
}