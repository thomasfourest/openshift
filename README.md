# openshift


## object run 

route - tls : 
service http -> route edge (avec redirect) 
service https avec son propre cert -> route passthrough

service :
clusterip 

label : oc label my-existing-label --overwrite

1 pod - plusieurs containers pouvant partager les volumes montés et sur meme reseau 127.0.0.1

oc scale --replicas=5 dc 

container image ? 

## objets build 

docker push : lookupPolicy > local true 

## cicd
2 types debuild config: 
- dockerfile 
- s2i (source2image)

buildConfig: 
output: to: kind: imageStreamTag (registry internal projet)
output: to: kind: dockerTag (registry private)


## secrets :
string: 
  data : valeurenclair
  
## trigger :
configchange
