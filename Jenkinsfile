
  
  [12:41] pravalikareddy6 (Guest)
pipeline {
agent any
environment {
dotnet=''
} stages {
stage('Checkout') {
steps {
}
}
stage('Restore') {
steps {
bat 'dotnet restore PATH'
}
}
stage('Clean') {
steps {
bat 'dotnet clean PATH'
}
}
stage('Build') {
steps {
bat 'dotnet build PATH --configuraton Release'
}
}
stage('Unit Test') {
steps {
bat 'dotnet test PATH'
}
}
stage('Publish') {
steps {
bat 'dotnet publish PATH'
}
}
stage('Versioning') {
steps {
}
}
stage('Zipfile') {
steps {
bat 'dotnet publish PATH'
}
stage('Uploading') {
steps {
bat 'aws s3 cp . s3://my-bucket/path --include "*.txt'
}
}
}
}
}


      
