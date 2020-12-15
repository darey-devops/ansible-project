pipeline {
    agent any

    parameters {
      string(name: 'inventory_file', defaultValue: 'dev',  description: 'This is the inventory file for the environment to deploy configuration')
      string(name: 'limit_inventory_group', defaultValue: '',  description: 'This is a group from the inventory file')
      string(name: 'ansible_tag', defaultValue: '', description: 'Ansible tag to only run specific tasks')
    }

//  environment {
//       JENKINS_SSH_PRIVKEY="~/.ssh/jenkins.pem"
//       JENKINS_KUBE_CONFIG_FILE="~/.kube/config"
//       JENKINS_ANSIBLE_CFG_FILE="${WORKSPACE}/playbooks/ansible.cfg"
//       ANSIBLE_FORCE_COLOR="true"
DEFAULT_PRIVATE_KEY_FILE
//     }

//     stages {

//         stage("Initial cleanup") {
//           steps {
//             dir("${WORKSPACE}") {
//               deleteDir()
//             }
//           }
//         }


//     stage('Checkout')
//         {
//         steps {
//         checkout([
//             $class: 'GitSCM', 
//             doGenerateSubmoduleConfigurations: false, 
//             extensions: [],
//             submoduleCfg: [], 
//             branches: [[name: 'develop']],
//             userRemoteConfigs: [[url: "https://gitlab.com/zooto.io/ansible.git",credentialsId:'GIT_CREDENTIALS']]
//             ])
//                 }
//           }

//         stage('Ansible playbook') {
//           steps {
//             script {
//               wrap([$class: 'AnsiColorBuildWrapper', 'colorMapName': 'XTerm']) {
//                 dir("${WORKSPACE}/playbooks") {
//                   sh("""#!/bin/bash -e
//                       # Prepare ansible options
//                       [ -n "\${ansible_tag}" ] && ansible_tag="--tags \${ansible_tag} "
//                       [ -n "\${limit_inventory_group}" ] && limit_inventory_group="--limit \${limit_inventory_group} "
//                       [ -n "\${inventory_file}" ] && inventory_file="-i ../inventory/\${inventory_file}"
                      
//                       set -x
//                       export ANSIBLE_CONFIG=${env.JENKINS_ANSIBLE_CFG_FILE}

//                       if [ ! -d "/var/lib/jenkins/.ansible/collections/ansible_collections/community/kubernetes" ] 
//                       then
//                       echo "Installing Required Ansible Collections"
//                       ansible-galaxy collection install -r ${WORKSPACE}/dependencies/requirements.yml --force 
//                       else
//                       echo "Ansible Collections already installed"
//                       fi

//                       ansible-playbook  \${inventory_file} \${limit_inventory_group} \${ansible_tag} site.yml --key-file ${env.JENKINS_SSH_PRIVKEY} --diff -vv
//                       set +x
                      
//                   """.stripIndent().trim())
//                 }
//               }
//             }
//           }      
//         }

//         // wrappers {
//         //   buildUserVars()
//         // }

//         stage("Final cleanup") {
//           steps {
//             dir("${WORKSPACE}") {
//               deleteDir()
//             }
//           }
//         }

//     }
}



