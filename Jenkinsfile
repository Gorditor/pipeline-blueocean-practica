pipeline {
  agent any
  stages {
    stage('Inicio') {
      steps {
        echo 'INICIO'
        bat(script: 'echo', encoding: 'Empezando pipeline...')
      }
    }

    stage('Sistema') {
      steps {
        echo 'SISTEMA'
        bat(script: 'echo', encoding: '%DATE% %TIME%')
      }
    }

    stage('Aprobation') {
      steps {
        input(message: '¿Continuar a FIN?', ok: 'Continuar')
      }
    }

    stage('Fin') {
      steps {
        echo 'FIN'
      }
    }

  }
}