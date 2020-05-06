node{
stage("SCM Checkout"){
git 'https://github.com/yogesh6717/Second_Maven_Project'
}
stage("Compile-Package"){
  def mvnHome = tool name: 'Maven', type: 'maven'
  sh "${mvnHome}/bin/mvn"
}
}
