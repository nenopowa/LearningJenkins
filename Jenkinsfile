def clima = "Hay tormenta"
del poblacion = 250000
pipeline{
  agent any
  stages{
    stage("Clima"){
      steps{
        println "La climatología actual en Vitoria-Gasteiz es: ${clima}"
      }
    }
    stage("Poblacion"){
      steps{
        println "Actualmente Vitoria-Gasteiz tiene una población de: ${poblacion} habitantes"
      }
    }
    stage("PobNeta"){
      steps{
        script{
          PoblacionNeta('Output')
        }
      }
    }
  }
}
def PoblacionNeta(String a)
{
  def neta = poblacion / 2
  echo "Poblacion neta actual: ${neta}"
}
