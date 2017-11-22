# CoCoSpoon

<p align="center">
<img width="10%" src="https://github.com/maxcleme/OPL-Rendu2/blob/master/report/images/logoCoCoSpoon.png" />
</p>
La couverture de code est une métrique représentant le pourcentage de code exécuté. Cette métrique est utiliser lors l'exécution de suites de tests afin de mesurer le code couvert par ces suites. 

Certaines méthodes de développement comme le TDD vont garantir une bonne couverture de par le fait que les tests sont écrit avant le code. Une question peut alors se poser, la totalité du code couvert est il bien exécuté en production ? Il est probable qu’une ligne de code exécuté lors d’une suite de tests, ne soit jamais exécutée dans un environnement de production. 

Le but est de montrer que calculer la couverture de code sur un programme exécuté dans un environnement de production est possible, de plus, ce calcul pourrait être réalisé en temps réel pour ne pas avoir à stopper l’exécution du code en production afin d’obtenir cette fameuse métrique.

Pour atteindre notre objectif, nous avons utiliser une librairie permettant de faire de la transformation de code source. L’idée est que le programme transformé puisse d’auto-instrumenter afin de notifier l’utilisateur de sa couverture à n'importe quel moment de son exécution.


# Usage

## CLI
    CocoSpoon
       -i, --input-path     input project folder
       -o, --output-path    instrumented project destination
      [-c, --classpath      classpath] 

## Maven

```xml
<dependencies>
    <dependency>
        <groupId>fil.iagl.cocospoon</groupId>
        <artifactId>CocoSpoon</artifactId>
        <version>1.0.0-SNAPSHOT</version>
    </dependency>
</dependencies>
<repositories>
    <repository>
        <id>tdurieux.github.io/maven-repository/snapshots/</id>
        <name>tdurieux.github.io maven-repository</name>
        <url>https://tdurieux.github.io/maven-repository/snapshots/</url>
    </repository>
</repositories>
```
# GUI

The GUI is availaible on <https://github.com/SpoonLabs/CoCoSpoon-ui>

# Screencast

[![alt tag](https://github.com/maxcleme/OPL-Rendu2/blob/master/report/images/youtubeVideo.png)](https://youtu.be/QUZK3erdiEM)


# Screenshots

![alt tag](https://github.com/maxcleme/OPL-Rendu2/blob/master/report/images/overall_view.png)
![alt tag](https://github.com/maxcleme/OPL-Rendu2/blob/master/report/images/package_view.png)
![alt tag](https://github.com/maxcleme/OPL-Rendu2/blob/master/report/images/couverture_classe.png)
