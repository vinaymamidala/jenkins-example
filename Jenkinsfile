node
{
def mavenHome = tool name: "maven3.6.2"

stage('Build')
{
 sh "${mavenHome}/bin/mvn clean package"
}
}
