node
{
def mavenHome = tool name: "maven3.6.3"

stage('Build')
{
 sh "${mavenHome}/bin/mvn clean package"
}
}
