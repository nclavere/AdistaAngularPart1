# Adista Angular #1
Formation de démarrage sur Angular pour débutants


## Install des outils

- Vérifier la version de node : ``node --version``
- Installer Angular CLI : ``npm install -g @angular/cli``
- Vérifier la version : ``ng version``
- Mémo des commandes Angular : https://gist.github.com/VikashSaharan1/e5b7dfd3b3084a1385270e8896aa7174

## Création d'une application Angular

```
ng new appTest
cd appTest
code .
```

Pour démarrer l'application, dans le terminale de VsCode : ``ng serve``

## Tutoriel Angular 

Tutoriel en mode local : https://angular.dev/tutorials/first-app

### -> Créer un composant Accueil

Dans les composants, remplacer le template Html par : ``templateUrl: './app.component.html'``


### -> Créer une interface

```Typescript
//Exemple d'interface et de classe
export interface IMyObject {
  id: number;
  label: string;
}

export class MyObject implements IMyObject {
  public id: number;
  public label: string;

  public constructor(id: number, label: string) {
    this.id = id;
    this.label = label;
  }

  public get shortlabel(): string {
    return this.label.substring(0, 32);
  }
}
```

### -> Utilisez *ngFor pour répertorier les objets du composant

Depuis Angular 17, on a une nouvelle  syntaxe de flux de contrôle : https://blog.angular-university.io/angular-for/

La documentation : https://angular.dev/guide/templates/control-flow

### -> Ajouter des itinéraires à l'application

A la fin : comparer avec le routing de l'application appTest ...

### -> Ajoutez la communication HTTP à votre application

Au lieu d'utiliser JSON Server : une petite API en C# ? 😉



