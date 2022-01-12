---
layout:     post
title:      "COLLECTION"
subtitle:   "Les premiers témoignages fossiles de l'activité de collection"
description: "
Les premiers témoignages fossiles de l'activité de collection sont recueillis par André Leroi-Gourhan lors de fouilles dans la grotte du Renne à Arcy-sur-Cure : des blocs de pyrite de fer, une coquille de gastéropode et un polypier fossiles sont volontairement apportés et gardés ensemble dans cette grotte habitée par l'homme de Neandertal au Moustérien1. Dans le monde grec et romain antique, des collections artistiques existent dans les temples (objets votifs), les bibliothèques …
"
excerpt: ""
date:       2021-04-16 15:00:00
author:     "Rabia"
image: "https://boremandjo.imgix.net/photo-1535905557558-afc4877a26fc.jpg"
published: true
tags:
    - Collection
    - Biblio
    - Sembura
categories: [ Revue de presse ]
URL: "/2018/04/16/using-helm-to-deploy-to-kubernetes/"
---

## Qu'est ce qu'une collection ?
- - -
Une collection est à la fois un regroupement d'objets correspondant à un thème, et l'activité qui consiste à réunir, entretenir et gérer ce regroupement.

## Histoire
- - -
Les premiers témoignages fossiles de l'activité de collection sont recueillis par André Leroi-Gourhan lors de fouilles dans la grotte du Renne à Arcy-sur-Cure : des blocs de pyrite de fer, une coquille de gastéropode et un polypier fossiles sont volontairement apportés et gardés ensemble dans cette grotte habitée par l'homme de Neandertal au Moustérien1.。

Dans le monde grec et romain antique, des collections artistiques existent dans les temples (objets votifs), les bibliothèques, dans les palais de princes hellénistiques ou auprès de lettrés. De nombreux épigrammes du papyrus de Milan décrivent ainsi des œuvres d'art ou des objets votifs (gemme, statue, ex-voto), affinant nos connaissances sur le regard ancien et sur la réception des images à l’époque hellénistique.

À la Renaissance, le cabinet de curiosités se répand dans le monde aristocratique européen, avec un certain goût pour l'hétéroclisme et l'inédit. L'engouement pour la collection à cette époque est appelé par les historiens italiens le collectionnisme3.

Krzysztof Pomian, l'un des pionniers de la recherche sur l'histoire des collections, définit la collection comme « tout ensemble d’objets naturels ou artificiels, maintenus temporairement ou définitivement hors du circuit d’activités économiques, soumis à une protection spéciale dans un lieu clos aménagé à cet effet et exposé au regard ». Ces objets perdent de leur utilité ou de leur valeur d'échange pour devenir « sémiophores », porteurs de sens4.

![](https://img.zhaohuabing.com/in-post/2018-04-16-using-helm-to-deploy-to-kubernetes/wordpress.png)


Collections：
* Collections scientifiques
* Collection d'œuvres d'art
* Collection d'objets de la vie quotidienne



## Collections scientifiques
- - -
Les collections scientifiques peuvent être constituées de spécimens d'histoire naturelle (botanique, zoologie, minéralogie, géologie, etc.), mais des objets se référant à toute autre discipline scientifique peuvent aussi les composer, comme des artéfacts d'archéologie, des cires anatomiques utilisées en médecine, des objets liés au génie et à la technique, etc.



## Collection d'œuvres d'art
- - -
Activité pratiquée d'abord par les aristocrates (exemple du mécénat), elle se développe par la suite dans la bourgeoisie (notamment dans le monde des artistes comme Étienne Moreau-Nélaton ou celui des affaires des années 1970). 

Elle peut se faire par plaisir ou par spéculation, suivre le conseil des critiques ou des marchands d'art pour faire son choix. L'amateur réunissant des œuvres d'art peut participer à des ventes aux enchères ou passer des commandes auprès des artistes, léguer parfois ses acquisitions à des institutions publiques.

* Collections scientifiques

* Collection d'œuvres d'art

* Collection d'objets de la vie quotidienne

* Collections scientifiques

* Collection d'œuvres d'art

* Collection d'objets de la vie quotidienne

>  Elle peut se faire par plaisir ou par spéculation, suivre le conseil des critiques ou des marchands d'art pour faire son choix. L'amateur réunissant des œuvres d'art peut participer à des ventes aux enchères ou passer des commandes auprès des artistes, léguer parfois ses acquisitions à des institutions publiques.
 
>  Elle peut se faire par plaisir ou par spéculation, suivre le conseil des critiques ou des marchands d'art pour faire son choix. L'amateur réunissant des œuvres d'art peut participer à des ventes aux enchères ou passer des commandes auprès des artistes, léguer parfois ses acquisitions à des institutions publiques.

Elle peut se faire par plaisir ou par spéculation, suivre le conseil des critiques ou des marchands d'art pour faire son choix. L'amateur réunissant des œuvres d'art peut participer à des ventes aux enchères ou passer des commandes auprès des artistes, léguer parfois ses acquisitions à des institutions publiques.

图2： Helm
![](https://img.zhaohuabing.com/in-post/2018-04-16-using-helm-to-deploy-to-kubernetes/helm-architecture.png)

## Collection d'objets de la vie quotidienne
- - -
La collection d'autoportraits du Corridor de Vasari, engagée par 200 tableaux par le cardinal Léopold de Médicis, la collection Verzocchi, collection originale de tableaux, autour du thème du travail, rassemblée à Forlì entre 1949 et 1950 par l'industriel italien Giuseppe Verzocchi, la collection Ares qui compte plusieurs collection d'artistes modernes et contemporain, la Collection Kesauri, appartenant à la famille Kesauri, des travaux de peintres connus qui déterminent le développement de l'art, de la Renaissance à nos jours sont des exemples de collections d'œuvres d'art.

1. Arénophile : collectionneur de sables
1. Arctophile : collectionneur d'ours en peluche
1. Bibliophile : collectionneur de livres

Appellation des collectionneurs par type de collection

```bash
Helm init
```

## Notes et références
- - -

Guy Buisson, Homo Collector, une anthropologie du collectionneur, éditions Amalthée, 2019.

```



```
helm create testapi-chart
```


```Bash
testapi-chart
├── charts
├── Chart.yaml
├── templates
│   ├── deployment.yaml
│   ├── _helpers.tpl
│   ├── NOTES.txt
│   └── service.yaml
└── values.yaml
```



```
apiVersion: v1
description: A simple api for testing and debugging
name: testapi-chart
version: 0.0.1
```


```
replicaCount: 2
image:
  repository: daemonza/testapi
  tag: latest
  pullPolicy: IfNotPresent
service:
  name: testapi
  type: ClusterIP
  externalPort: 80
  internalPort: 80
resources:
  limits:
    cpu: 100m
    memory: 128Mi
  requests:
    cpu: 100m
    memory: 128Mi
```


```
helm lint
==> Linting .
[INFO] Chart.yaml: icon is recommended

1 chart(s) linted, no failures
```



```
helm package testapi-chart --debug
```


```
Saved /Users/daemonza/testapi/testapi-chart/testapi-chart-0.0.1.tgz to current directory
Saved /Users/daemonza/testapi/testapi-chart/testapi-chart-0.0.1.tgz to /Users/daemonza/.helm/repository/local
```



## Bibliographie
- - -
Enrico Castruccio, I Collezionisti usi, costumi, emozioni, Cremona, Persico Edizioni, 2008 (ISBN 88-87207-59-3)
```
helm search testapi
No results found
```



Enrico Castruccio, I Collezionisti usi, costumi, emozioni, Cremona, Persico Edizioni, 2008 (ISBN 88-87207-59-3)
```Bash
helm repo list
NAME    URL
stable  https://kubernetes-charts.storage.googleapis.com
```

Enrico Castruccio, I Collezionisti usi, costumi, emozioni, Cremona, Persico Edizioni, 2008 (ISBN 88-87207-59-3)

```Bash
helm serve&
Now serving you on 127.0.0.1:8879
```
Enrico Castruccio, I Collezionisti usi, costumi, emozioni, Cremona, Persico Edizioni, 2008 (ISBN 88-87207-59-3)
```Bash
helm repo add local http://127.0.0.1:8879
"local" has been added to your repositories
```
Enrico Castruccio, I Collezionisti usi, costumi, emozioni, Cremona, Persico Edizioni, 2008 (ISBN 88-87207-59-3)

```Bash
helm search testapi

NAME                    CHART VERSION   APP VERSION     DESCRIPTION
local/testapi-chart     0.0.1                           A Helm chart for Kubernetes
```

## Article connexe
- - -
Enrico Castruccio, I Collezionisti usi, costumi, emozioni, Cremona, Persico Edizioni, 2008 (ISBN 88-87207-59-3)
```
 helm install local/testapi-chart --name testapi
```
Article connexe

```
NAME:   testapi
LAST DEPLOYED: Mon Apr 16 10:21:44 2018
NAMESPACE: default
STATUS: DEPLOYED

RESOURCES:
==> v1/Service
NAME                   TYPE       CLUSTER-IP    EXTERNAL-IP  PORT(S)  AGE
testapi-testapi-chart  ClusterIP  10.43.121.84  <none>       80/TCP   0s

==> v1beta1/Deployment
NAME                   DESIRED  CURRENT  UP-TO-DATE  AVAILABLE  AGE
testapi-testapi-chart  1        1        1           0          0s

==> v1/Pod(related)
NAME                                   READY  STATUS   RESTARTS  AGE
testapi-testapi-chart-9897d9f8c-nn6wd  0/1    Pending  0         0s


NOTES:
1. Get the application URL by running these commands:
  export POD_NAME=$(kubectl get pods --namespace default -l "app=testapi-testapi-chart" -o jsonpath="{.items[0].metadata.name}")
  echo "Visit http://127.0.0.1:8080 to use your application"
  kubectl port-forward $POD_NAME 8080:80
```

Enrico Castruccio, I Collezionisti usi, costumi, emozioni, Cremona, Persico Edizioni,
```
helm ls
```

Article connexe
```
NAME    REVISION        UPDATED                         STATUS          CHART                   NAMESPACE
testapi 1               Mon Apr 16 10:21:44 2018        DEPLOYED        testapi-chart-0.0.1     default
```

