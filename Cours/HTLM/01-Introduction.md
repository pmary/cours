# HTML

## Qu'est-ce que le HTML ?
Le HTML est un langage de balisage que l'on utilise pour formater du contenu dans un documents HTML. Le contenu ainsi formaté représente une page web.  
Mais qu'est-ce que ça veut dire de "baliser" un document au juste ? Et bien quand vous étiez au collège, votre prof de français insistait sans doute pour que vous souligniez vos titres d'une certaine façon, les titre de chapitre d'une autre, les sous titres en bleu etc... Vous balisiez alors votre document suivant une norme qui le rendait interprétable par votre professeur. Ici, le professeur, c'est le navigateur web, et la norme pour baliser le document est l'HTML.  
Une fois qu'on a dit ça, qu'est-ce qu'une balise ?  

## Les balises
Une balise, c'est une instruction à destination du navigateur. Il en a besoin pour pouvoir interpréter votre document et la nature du texte qu'elles contiennent. Concrétement, une balise est un mot entouré de "chevrons", vous savez, ces symboles `<` et `>`. Une balise ressemble donc à ceci : `<h1>`. _On reviendra plus tard sur la signafication sémantique des balises, pour le moment sachez juste qu'une balise "h1" indique un titre de niveau 1 (Header 1)_.  
Il y a deux types de balises : Celles qui vont par paires et les balises orphelines (ou auto-fermantes).  

### Les balises en paires
Prenons l'exemple de la balise h1, qui est une balise en paire:  
```html
Pas un titre
<h1>Mon titre</h1>
Pas un titre
```
On appel la balise `<element>` une balise ouvrante et `</element>` une balise fermante. En l'occurence, pour indiquer au navigateur que le texte "Mon titre" doit être interprété comme un titre de niveau 1, je le met entre une balise ouvrante `<h1>` et sa contrepartie obligatoire, la balise fermante `</h1>`. En résumé, on ouvre pour indiquer ou commence le titre et ou il se termine.

### Les balises orphelines
C'est une balise qui permet d'insérer un élément, comme une image ou une vidéo. Comme elle ne sert pas à délimiter un contenu, elle se ferme toute seule, comme ceci :  
```html
<img />
```
_`img` (pour image) est le nom de la balise permettant d'insérer une image._  

### Les attributs
Les attributs viennent donner plus d'informations aux balises. Un attribut se place toujours dans la ouvrante :  
```html
<balise attribut>
```

Il peut également avoir une valeur, auquel cas la syntaxe sera toujours le nom de l'attribut suivant du symbole =, suivit de la valeur de l'attribut entre guilleter `"`, le tout sans expace, comme ceci :  
```html
<balise attribut="valeur">
```

Les usages sont nombreux. Par exemple, si l'on souhaite insérer une image nous devons indiquer laquelle. C'est le rôle de l'attribut `src` (pour source) :  
```html
<img src="oiseau.jpg" />
```

Notez que certains attributs sont réservés à certaines balises, par exemple, l'attribut `src` n'est pas utilisable sur une balise `<h1>`.

## Structure de base d'une page HTML5
Une page HTML5 a une structure de base qui est obligatoire, la voici :  

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8" />
        <title>Titre</title>
    </head>

    <body>
    
    </body>
</html>
```