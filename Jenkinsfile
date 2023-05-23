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
    stage('ssh0'){
  sshPut remote: remote, from: 'hasee99.sh', into: '/home/opc'
 }
  stage('ssh1'){
 sshCommand remote: remote, command: "sudo sh /home/opc/hasee99.sh"
 }
  stage('ssh2'){
 sshCommand remote: remote, command: "pwd"
 }
  stage('ssh3'){
 sshCommand remote: remote, command: "mv /home/opc/hasee99 /home/opc/hasee99/"
 }
}
