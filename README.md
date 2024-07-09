# gitops

Projeto com gitops

Automatizando deploy com GITOPS e GITACTIONS

sed -i 's/image: rfahham\/workon:[0-9].[0-9].[0-9]\{1,3\}/image: rfahham\/workon:v${{github.run_number}}/' ./k8s/deployment.yaml
        
sed -i 's/image: rfahham\/workon:2.0.0/image: rfahham\/workon:v${{github.run_number}}/' ./k8s/deployment.yaml