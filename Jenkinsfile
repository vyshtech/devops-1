node(){
stage("prepare"){
  git "https://github.com/sixlog/devops.git"
}
stage("ansiblke-playbook"){
ansible -i host all -m ping
}
stage("dev stage")
{
 ansible-playbook -i hosts site.yml
}
  stage("slck notification") {
   slack.notify("channel: name") 
  }

}
def slacknotification(){
  
}
