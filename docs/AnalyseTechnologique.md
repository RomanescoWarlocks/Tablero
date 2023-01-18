Ce document décrit une comparaison des technologies pour développer une application Desktop sur Windows ce qui aboutira à un choix pour développer le projet. Il ne sera considéré ici que les technologies se basant sur dotNet.

# Frameworks pour l'UI
Il sera question ici de choisir le framework utilisé pour l'interface graphique
## Frameworks dépréciées

### WinForms
WinForms (ou Windows Forms) a été pendant longtemps la technologie par défaut pour du développement Windows en dotNET. Le projet est cependant en mode maintenance depuis 2014 donc sans ajout de fonctionnalités depuis. Il a donc été décidé de partir sur des technologies plus moderne.

## Framework actuels
Windows propose plusieurs solutions de développement dotNet pour une app Desktop dorénavant. Les principales étant WPF, WinUI et MAUI.

### WPF
WPF (Windows Presentation Forms) est actuellement la librairie la plus utilisé pour les apps Desktop. C'est un framework avec beaucoup de ressources disponible, le framework étant disponible depuis 2006. La façon de créer interface utilisateur s'apparente à la façon classique de développer l'UI dans Android, c'est à dire un fichier dans un langage de balisage (ici XAML) décrivant la structure de l'UI et un fichier de code permettant de lier les éléments graphiques aux données.

### WinUI

WinUI (Windows UI) est un framework alternatif à WPF. Il fonctionne de manière relativement similaire à WPF mais propose des designs plus modernes que WPF car il suit le [Fluent Design System](https://www.microsoft.com/design/fluent/) qui sont des règles de design applicables aux apps Windows. Cependant étant plus récent que WPF, il dispose de moins de ressources disponibles que ce dernier en termes de librairies et de support.

### MAUI
.NET Multi-platform App UI (MAUI) est la solution moderne de Microsoft pour des apps cross-platform (PC, Mac, Android, IOS). On peut le considérer comme le Flutter de Microsoft. Pour les applications Windows car c'est le target du projet, MAUI se repose sur WinUI.

# Choix du framework

Il a été décidé d'écarter MAUI car dans le cadre du projet, il n'y a pas besoin d'avoir du cross-platform ce qui ajouterait des contraintes inutiles. Le choix a du donc se faire entre WPF et WinUI. Les deux sont relativement similaires mais le choix a été de partir sur WPF pour la raison que dû à son ancienneté, plus de ressources sont disponibles que pour WinUI, aussi l'interface du projet étant relativement simple, il n'y a pas forcément besoin d'avoir une UI dernier cri.

WPF sera donc le framework UI utilisé.

# Langages

Avec le choix de WPF, cela restreint forcément le choix du langage. Les deux choix principaux sont C# et F#. C# est le langage orienté objet classique de dotNet tandis que F# est son pendant fonctionnel.
C# a été choisi purement par préférence personnelle car je suis plus à l'aise avec de l'orienté objet que du fonctionnel
