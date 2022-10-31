[Article Wikipedia - C++](https://fr.wikipedia.org/wiki/C%2B%2B)
[^comment]: Le project Markdown sert a démontrer notre habilité à utiliser ce langue de Markup. 
# C++
---
C++ est un [langage de programmation](https://fr.wikipedia.org/wiki/Langage_de_programmation) [compilé](https://fr.wikipedia.org/wiki/Compilateur) permettant la programmation sous de multiples [paradigmes](https://fr.wikipedia.org/wiki/Paradigme_(programmation)), dont la [programmation procédurale](https://fr.wikipedia.org/wiki/Programmation_proc%C3%A9durale), la [programmation orientée objet](https://fr.wikipedia.org/wiki/Programmation_orient%C3%A9e_objet) et la [programmation générique](https://fr.wikipedia.org/wiki/G%C3%A9n%C3%A9ricit%C3%A9). Ses bonnes performances, et sa compatibilité avec le C en font un des langages de programmation les plus utilisés dans les applications où la performance est critique.

Créé initialement par [Bjarne Stroustrup](https://fr.wikipedia.org/wiki/Bjarne_Stroustrup) dans les années 1980, le langage C++ est aujourd'hui normalisé par l'ISO. Sa première normalisation date de 1998 (ISO/CEI 14882:1998), ensuite amendée par l'erratum technique de 2003 (ISO/CEI 14882:2003). Une importante mise à jour a été ratifiée et publiée par l'ISO en septembre 2011 sous le nom de ISO/IEC 14882:2011, ou C++113. Depuis, des mises à jour sont publiées régulièrement : en 2014 (ISO/CEI 14882:2014, ou C++144), en 2017 (ISO/CEI 14882:2017, ou C++175) puis en 2020 (ISO/IEC 14882:2020, ou C++206).

![Bjarne Stroustrup, l'inventeur du C++.](BjarneStroustrup.jpg)
*Bjarne Stroustrup, l'inventeur du C++.*
## Dénomination
---
En [langage C](https://fr.wikipedia.org/wiki/C_(langage)), `++` est l'opérateur d'incrémentation, c'est-à-dire l'augmentation de la valeur d'une variable de 1. C'est pourquoi C++ porte ce nom : cela signifie que C++ est un niveau au-dessus de C.

## Histoire
---
**Bjarne Stroustrup** commence le développement de C *with Classes* (C avec classes) en 19797. Il travaille alors dans les laboratoires Bell où il est notamment collègue de l'inventeur du C *Dennis Ritchie*. L'idée de créer un nouveau langage venait de l'expérience en programmation de Stroustrup pour sa thèse de doctorat. Il s'agissait en l'occurrence d'améliorer le langage C. Stroustrup trouvait que Simula avait des fonctionnalités très utiles pour le développement de gros programmes mais qu'il était trop lent pour être utilisé en pratique (cela était dû à un problème d'implémentation du compilateur Simula), tandis que BCPL était rapide mais de trop bas niveau et non adapté au développement de gros logiciels. Quand Stroustrup commença à travailler aux laboratoires Bell, on lui demanda d'analyser le noyau UNIX en vue de faire du calcul distribué. Se rappelant sa thèse, Stroustrup commença à améliorer le langage C avec des fonctionnalités similaires à celle de Simula. C fut choisi parce qu'il est rapide, portable et d'usage général. En outre, il était une bonne base pour le principe original et fondateur de C++ : « vous ne payez pas pour ce que vous n'utilisez pas ». Dès le départ, le langage ajoutait à C la notion de classe (avec encapsulation des données), de classe dérivée, de vérification des types renforcés (typage fort), d'« inlining », et d'argument par défaut.

Alors que Stroustrup développait C *with classes*, il écrivit CFront, un compilateur qui générait du code source C à partir de code source C *with classes*. La première commercialisation se fit en octobre 1985. En 1983 le nom « C++ » est inventé, et en 1984 le nom du langage passa de C *with classes* à celui de « C++ ». Parmi les nouvelles fonctionnalités qui furent ajoutées au langage, il y avait les fonctions virtuelles, la surcharge des opérateurs et des fonctions, les références, les constantes, le contrôle du typage amélioré et les commentaires en fin de ligne. En 1985 fut publiée la première édition de The C++ Programming Language, apportant ainsi une référence importante au langage qui n'avait pas encore de standard officiel. En 1989, c'est la sortie de la version 2.0 de C++. Parmi les nouvelles fonctionnalités, il y avait l'héritage multiple, les classes abstraites, les fonctions membres statiques, les fonctions membres constantes, et les membres protégés. En 1990, The Annotated C++ Reference Manual (« ARM ») fut publié apportant les bases du futur standard. Les ajouts de fonctionnalités tardifs qu'il comportait couvraient les templates, les exceptions, les espaces de noms, les nouvelles conversions et le type booléen.

Pendant l'évolution du langage C++, la bibliothèque standard évoluait de concert. Le premier ajout à la bibliothèque standard du C++ concernait les flux d'entrées/sorties qui apportaient les fonctionnalités nécessaires au remplacement des fonctions C traditionnelles telles que `printf` et `scanf`. Ensuite, parmi les ajouts les plus importants, il y avait la Standard Template Library. Après des années de travail, un comité réunissant l'ANSI et l'ISO standardisa C++ en 1998 (ISO/CEI 14882:1998), l'année où le comité de standardisation se réunissait à Sophia Antipolis dans le sud de la France. Pendant quelques années après la sortie officielle du standard, le comité traita des problèmes remontés par les utilisateurs, et publia en 2003 une version corrigée du standard C++.

Personne ne possède le langage C++. Il est libre de droits8 ; cependant, le document de standardisation n'est quant à lui pas disponible gratuitement.

## Fonctionnalités introduites
---
On peut considérer que C++ « est du C » avec un ajout de fonctionnalités. Cependant, plusieurs programmes syntaxiquement corrects en C ne le sont pas en C++, à commencer bien sûr par ceux qui font usage d'identificateurs correspondant à des mots-clefs en C++.

Parmi les fonctionnalités ajoutées figurent :

- le typage des « prototypes » de fonctions (repris dans ANSI C89) ;
- La surcharge des fonctions ;
- les déclarations reconnues comme instructions (repris dans C99) ;
- les opérateurs `new` et `delete` pour la gestion d'allocation mémoire ;
- le type de données `bool` (booléen) ;
- les références `&` 9;
- les variables et les fonctions membres `const` (repris partiellement par C à la fin des années 1980) ;
- les fonctions `inline` (repris dans C99) ;
- les paramètres par défaut dans les fonctions ;
- les référentiels lexicaux (espaces de noms) et l'opérateur de résolution de portée :: ;
- les classes, ainsi que tout ce qui y est lié : l'héritage, les fonctions membres, les fonctions membres virtuelles, les constructeurs - et le destructeur ;
- la surcharge des opérateurs ;
- les templates ;
- la gestion d'exceptions ;
- l'identification de type pendant l'exécution (RTTI : run-time type information) ;
- le commentaire sur une ligne introduit par `//` (existant dans BCPL, repris dans C99) ;
- les références de rvalue `&&` (C++11) ;
- la déduction de type à la compilation via `auto` (C++11) ;
- les expressions constantes `constexpr` (C++11)10;
- les fonctions lambda (C++11, étendu dans tous les standards publiés depuis) ;
- les boucles for basées sur une plage (C++11, étendu en C++20) ;
- les modules via `import`, `export` et `module` (C++20) ;
- les contraintes et concepts via `concept` et `requires` (C++20) ;
- les fonctions immédiates `consteval` (C++20) ;
- les coroutines (C++20) ;

La compilation d'un programme en C++ effectue également un contrôle plus minutieux du typage.

## Bibliothèque standard
---
La bibliothèque standard du C++ englobe la ***Standard Template Library (STL)*** qui met à la disposition du programmeur des outils puissants comme des collections (conteneurs) et des itérateurs.

À l'origine, la STL était une bibliothèque développée par Alexander Stepanov qui travaillait pour Hewlett-Packard. Dans la norme, celle-ci n'est pas appelée STL, car elle est considérée comme faisant partie de la bibliothèque standard de C++. Toutefois, beaucoup de personnes l'appellent encore de cette manière pour distinguer d'une part, les fonctions d'entrées/sorties comprises dans cette bibliothèque et, d'autre part, celles fournies par la bibliothèque C.

Comme en C, l'utilisation d'une bibliothèque peut se faire par l'intermédiaire de la directive `#include` (suivie du nom du fichier d'en-tête), et certaines d'entre elles (`cmath`, `thread`, etc.) nécessitent d'être liées explicitement. Depuis C++20 le mot clé `import` peut servir à des fins similaires.

## Programmation orientée objet
---
Le langage C++ utilise les concepts de la programmation orientée objet et permet entre autres :

![Exemple de hiérarchie de classes type stream.](https://upload.wikimedia.org/wikipedia/commons/thumb/f/fb/Stream_class_Hierarchy.tif/lossless-page1-330px-Stream_class_Hierarchy.tif.png)
*Exemple de hiérarchie de classes type stream.*
- la création de classes ;
    - l'encapsulation ;
    - des relations entre les classes :
        - la composition de classes (composition dans un diagramme de classes),
        - l'association de classes (en) (association dans un diagramme de classes),
        - l'agrégation de classes (agrégation dans un diagramme de classes),
        - la dépendance (dépendance dans un diagramme de classes),
        - l'héritage simple et multiple (héritage dans un diagramme de classes) ;
- le polymorphisme ;
- l'abstraction ;
- la généricité ;
- la méta-programmation.

## Encapsulation
---
L'encapsulation permet de faire abstraction du fonctionnement interne (c'est-à-dire, la mise en œuvre) d'une classe et ainsi de ne se préoccuper que des services rendus par celle-ci. C++ met en œuvre l'encapsulation en permettant de déclarer les membres d'une classe avec le mot réservé `public`, `private` ou `protected`. Ainsi, lorsqu'un membre est déclaré :

- `public`, il sera accessible depuis n'importe quelle fonction ;
- `private`, il sera uniquement accessible d'une part, depuis les fonctions qui sont membres de la classe et, d'autre part, depuis les fonctions autorisées explicitement par la classe (par l'intermédiaire du mot réservé `friend`) ;
- `protected`, il aura les mêmes restrictions que s'il était déclaré `private`, mais il sera en revanche accessible par les classes filles.
  
C++ n'impose pas l'encapsulation des membres dans leurs classes. On pourrait donc déclarer tous les membres publics, mais en perdant une partie des bénéfices apportés par la programmation orientée objet. Il est de bon usage de déclarer toutes les données privées, ou au moins protégées, et de rendre publiques les fonctions membres agissant sur ces données. Ceci permet de cacher les détails de la mise en œuvre de la classe.

## « Hello, world »
---
Voici l'exemple de Hello world donné dans The C++ Programming Language, Third Edition de Bjarne Stroustrup :
```c++
#include<iostream>

int main()
{
    std::cout << "Hello, new world!\n";
}
```

Dans l'exemple ci-dessus, le code source `std::cout << "Hello, new world!\n"` envoie la chaîne de caractères `"Hello, new world!\n"` à l'objet global `cout`, défini dans l'espace de noms standard `std`, grâce à l'opérateur `<<` de `cout`.

### Espace de noms
---
En C++, le mot clef namespace permet de définir et de nommer des espaces de noms (namespaces), notion déjà présente en langage C ; en effet, le corps d'une routine, d'une structure de contrôle de flux d'exécution, d'une structure de données ou d'une section de code (délimitée par les accolades { et }) constitue un espace de noms. En C++, le corps d'une classe, à l'instar du corps d'une structure de données, constitue aussi un espace de noms.

Dans différents espaces de noms, on peut ainsi définir des entités (routines, variables, etc.) ayant le même identificateur. L'ambiguïté est résolue en utilisant le nom de l'espace de nom devant l'opérateur de portée (::) pour indiquer l'espace de noms dans lequel on veut accéder. Notez que l'espace de noms global du programme n'a pas de nom. Pour accéder à une entité globale, cachée par une entité locale par exemple, on utilise l'opérateur de portée précédé d'aucun nom.

## Directive « using »
---
Il est possible de spécifier un espace de noms précis à utiliser afin d'éviter d'avoir à recourir à l'opérateur de résolution de portée. Pour cela, le mot-clé using est utilisé avec cette syntaxe :

```c++
using namespace nom_du_namespace;
// ou
using nom_d_un_symbole;
// ou
using enum nom_d_un_enum_class; // C++20
```
Ainsi, pour utiliser la variable cout définie dans le namespace standard sans utiliser l'opérateur de résolution de portée, il est possible d'écrire using namespace std; ou using std::cout;. Cela est valable pour tous les espaces de noms. Cette instruction se place en général avant le début du code source proprement dit :

```c++
#include <iostream>
using namespace std;

int main()
{
    cout << "Hello, new world!\n";
}
```
Il est aussi possible, et conseillé, d'importer un symbole particulier, ou de placer cette instruction dans une fonction afin de limiter la portée :

```c++
#include <iostream>

int main()
{
    using std::cout;
    // std::cout est disponible sans utilisation de std::
    cout << "Hello, new world!" << std::endl; // mais pas std::endl (endline)
}

void foo()
{
    // std::cout n'est plus disponible sans utilisation de std::
    std::cout << "Hello, new world!" << std::endl;
}
```
Le mot-clé using peut aussi être utilisé dans les classes. Si une classe B hérite d'une classe A, elle peut grâce à ce mot-clé passer des membres protected de A en public dans B, ou encore démasquer une fonction membre de A qui le serait par une fonction membre de B de même nom :
```c++
#include <iostream> 

// Déclaration de la classe de base A.
class A
{
protected:
    void f()
    {
        std::cout << "A::f()\n";
    }

public:
    void g()
    {
        std::cout << "A::g()\n";
    }
};

// Déclaration de la classe B héritant de A.
class B : public A
{
public:
    using A::f; // rend public A::f()
};

// Déclaration de la classe C héritant de A.
class C: public A
{
public:
    void g(int Val) // masque A::g()
    {
        std::cout << "C::g(int)\n";
    }
};

// Déclaration de la classe D héritant de A.
class D: public A
{
public:
    void g(int Val) // masque A::g()
    {
        std::cout << "D::g(int)";
    }
    using A::g;      // démasque A::g()
};

int main()
{
    A a;
    B b;
    C c;
    D d;

    // a.f();  // impossible car f est protégé dans A
    a.g();

    b.f();  // possible car A::f est publique dans B.

    // c.g();  // impossible car A::g() est masquée par C::g(int) dans C
    c.g(6); // possible car C::g(int Val) est masquée par C::g(int) dans C

    d.g();  // possible car A::g() est démasquée dans D
    d.g(5); // possible car D::g() est démasquée dans D
}
```
Le programme ci-dessus affiche :

```c++
A::g()
A::f()
C::g(int)
A::g()
D::g(int)
```
Il est aussi possible de définir un nouveau nom pour un namespace :

>`namespace fs = std::filesystem;`
>`// on peut alors écrire fs::path au lieu de std::filesystem::path`


## Déclaration et définition de classe
---
Il est d'usage de séparer prototype (déclaration) et implémentation (définition) de classe dans deux fichiers : la déclaration se fait dans un fichier d'en-tête (dont l'extension varie selon les préférences des développeurs : sans extension dans le standard, .h comme en C, .hh ou .hpp ou .hxx pour différencier le code source C++ du C) alors que la définition se fait dans un fichier source (d'extension également variable : .c comme en C, .cc ou .cpp ou .cxx pour différencier C++ du C).

### Déclaration de classe
---
Exemple de la déclaration d'une classe comportant des attributs privés et des fonctions membres publiques :

```c++
// messageinternet.hpp
#include <string_view>

class MessageInternet
{
private: // Ici, private: est optionnel car il est par défaut.
    std::string_view m_sujet;
    std::string_view m_expediteur;
    std::string_view m_destinataire; // attributs
    
public:
    // constructeur
    MessageInternet(
        std::string_view sujet,
        std::string_view expediteur,
        std::string_view destinataire);
    // fonctions membres :
    auto sujet();
    auto expediteur();
    auto destinataire();
};
```

### Définition de classe
---
Le nom d'une fonction membre déclarée par une classe doit nécessairement être précédé du nom de la classe suivi de l'opérateur de résolution de portée 
`::`.
Exemple de définition des fonctions membres d'une classe (celle déclarée précédemment) :
```c++
// messageinternet.cpp
#include "messageinternet.hpp"

MessageInternet::MessageInternet(
    std::string_view sujet,
    std::string_view expediteur,
    std::string_view destinataire)
        : m_sujet(sujet),
          m_expediteur(expediteur),
          m_destinataire(destinataire)
    {}

auto MessageInternet::sujet() { return m_sujet; }
auto MessageInternet::expediteur() { return m_expediteur; }
auto MessageInternet::destinataire() { return m_destinataire; }
```
##  Références
---
1. (en) Bjarne Stroustrup, Bjarne Stroustrup's FAQ : FAQ de Bjarne Stroustrup, www.stroustrup.com, modified february 2, 2012. (lire en ligne)
2. « ISO/IEC 14882:2020 Programming languages — C++ », décembre 2020
3. ISO/IEC 14882 : 2011 : Technologies de l'information -- Langages de programmation -- C++, ISO, 1er septembre 2011 (présentation en ligne)
4. ISO/IEC 14882 : 2014 : Technologies de l'information -- Langages de programmation -- C++, ISO, 15 décembre 2014 (présentation en ligne)
5. ISO/IEC 14882 : 2017 : Technologies de l'information -- Langages de programmation -- C++, ISO, décembre 2017 (présentation en ligne)
6. 14:00-17:00, « ISO/IEC 14882:2020 », sur ISO (consulté le 20 décembre 2020)
7. (en) Bjarne Stroustrup, A Tour of C++, Addison-Wesley, coll. « C++ In-Depth Series », 2018, 240 p. (ISBN 978-0-13-499783-4), 16.1.1 Timeline
8. « Programmation Langage C++ - Web-Libre.org », sur www.web-libre.org (consulté le 6 octobre 2020)
9. « Standard C++ », sur isocpp.org (consulté le 27 janvier 2022) : « References are useful for several things, but the direct reason they were introduced in C++ was to support operator overloading »
10. (en-US) corob-msft, « Welcome back to C++ - Modern C++ » , sur docs.microsoft.com (consulté le 21 décembre 2020)
11. The C++ Programming Language, Third Edition, chap. 1.1.1, page 5
12. (en) Jeff Snyder, Louis Dionne, « Class Types in Non-Type Template Parameters » , 6 juin 2018 (consulté le 12 mars 2021)
13. « Using the GNU Compiler Collection (GCC): Optimize Options », sur gcc.gnu.org (consulté le 11 mars 2019)
14. « CLion : A Cross-Platform IDE for C and C++ by JetBrains », sur JetBrains (consulté le 4 août 2020).
15. (en) Doug Schaefer, « Eclipse CDT | The Eclipse Foundation », sur www.eclipse.org (consulté le 4 octobre 2020)