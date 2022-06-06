# VINGARCH_Etude_longitudinale

Résultats d'étude réalisé lors d'un stage à l'INSERM concernant le calcul d'un estimateur clinique l'ATT ( Average treatment on the treated ) dans un contexte non randomisé et sans groupe de controle.  

### I) Contexte :

Dans le cadre d’une étude clinique longitudinale, la question de l’efficacité du
traitement est centrale. Il existe dans ce contexte différents indicateur permettant
d’y répondre, l’ATT ( average treatment effect on the treated ) en est un exemple im-
portant.
Comme son nom l’indique cet indicateur permet de calculer l’effet moyen d’un trai-
tement sur le groupe des individus qui ont été traités. Dans le cadre d’une étude non
randomisée cet indicateur peut être estimer à l’aide de méthodes statistiques.
L’une des méthodes est développée par Gran et al. dans l’article ”Estimating the
treatment effect on the treated under time-dependent confounding in an application
to the Swiss HIV Cohort Study”  
L'idée de l'article est d'apprendre un modèle sur l'évolution du risque chez les individuts non traitées puis d'utiliser ce modèle pour créer des variables contre-factuelles afin d'estimer l'efficacité du traitement.  
Plus précisément on apprend un modèle VAR ( Vectorial Autoregressive model ) sur les temps ou les individuts ne sont pas traitées et on en déduit des contrefactuelles pour les temps ou ces memes individuts sont traitées. Voici une image permettant de représenter la situation mentionné :  
![Image1](Img/contrefa.png)

### II) Restriction de l'article : 

Cet article se restreint a des covariables conti
