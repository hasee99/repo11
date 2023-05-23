node{
  def remote = [:]
  remote.name = 'oraclevm'
  remote.host = '152.67.160.182'
  remote.user = 'opc'
  remote.password = 'Muzammil073#'
  remote.allowAnyHosts = true
    stage('checkout') {
           checkout scm
  }  
    stage('ssh1'){
  sshPut remote: remote, from: 'hasee99.sh', into: '/home/opc'
 }
  stage('ssh2'){
 sshCommand remote: remote, command: "sudo sh /home/opc/hasee99.sh"
 }
  stage('ssh3'){
 sshCommand remote: remote, command: "pwd"
 }
  stage('ssh4'){
 sshCommand remote: remote, command: "mv /home/opc/hasee99.sh /home/opc/hasee99/"
 }
}

 
