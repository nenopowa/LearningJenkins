def clima = "Hay tormenta"
def poblacion = 250000
pipeline{
  agent any
  stages{
    stage("Clima"){
      steps{
        println "La climatologia actual en Vitoria-Gasteiz es: ${clima}"
      }
    }
    stage("Poblacion"){
      steps{
        println "Actualmente Vitoria-Gasteiz tiene una poblacion de: ${poblacion} habitantes"
      }
    }
    stage("PobNeta"){
      steps{
        script{
          PoblacionNeta(poblacion)
        }
      }
    }
  }
}
def PoblacionNeta(integer a)
{
  def neta = a / 2
  echo "Poblacion neta actual: ${neta}"
}
