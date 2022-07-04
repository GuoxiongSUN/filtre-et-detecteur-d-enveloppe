# 7.4

**Objectif** : Implémenter la détection d'enveloppe partielle pour les signaux chirp.

**Méthode** : La fréquence du signal chirp étant toujours croissante, un filtre permet de tronquer partiellement le signal chirp. Il est suivi d'un circuit de détection d'enveloppe, qui atteint finalement l'objectif.

![111.png](7%204%20674c023a6c0648f0addb10a3a8775e30/111.png)

**Détails spécifiques:**

Dans cette expérience, des filtres passe-bas RC du premier, deuxième et troisième ordre ont été construits dans le but de comparer les performances des filtres à différents ordres.
Et dans le test de données, les résultats générés par différents R et C dans le montage de détection d'enveloppe ont été examinés.

---

Circuits du premier ordre:

![222.png](7%204%20674c023a6c0648f0addb10a3a8775e30/222.png)

Circuits du deuxième ordre:

![8~99[ES1RN_ELBE22G$J5]U.png](7%204%20674c023a6c0648f0addb10a3a8775e30/899ES1RN_ELBE22GJ5U.png)

Circuits du troisième ordre:

![L6A330XG745CT%UIJU`8711.png](7%204%20674c023a6c0648f0addb10a3a8775e30/L6A330XG745CTUIJU8711.png)

Montage de détection d'enveloppe:

![7H6742D9[RZU%S71YXEU5]7.png](7%204%20674c023a6c0648f0addb10a3a8775e30/7H6742D9RZUS71YXEU57.png)

---

**Signal d'entrée:**

![Untitled](7%204%20674c023a6c0648f0addb10a3a8775e30/Untitled.png)

**Résultats des tests:**

C=1nF, R=24kΩ, Circuits du premier ordre

![Untitled](7%204%20674c023a6c0648f0addb10a3a8775e30/Untitled%201.png)

C=1nF, R=24kΩ, Circuits du deuxième ordre

![Untitled](7%204%20674c023a6c0648f0addb10a3a8775e30/Untitled%202.png)

C=1nF, R=24kΩ, Circuits du troisième ordre

![Untitled](7%204%20674c023a6c0648f0addb10a3a8775e30/Untitled%203.png)

C=1nF, R=240kΩ, Circuits du premier ordre

![Untitled](7%204%20674c023a6c0648f0addb10a3a8775e30/Untitled%204.png)

C=1nF, R=240kΩ, Circuits du deuxième ordre

![Untitled](7%204%20674c023a6c0648f0addb10a3a8775e30/Untitled%205.png)

C=1nF, R=240kΩ, Circuits du troisième ordre

![Untitled](7%204%20674c023a6c0648f0addb10a3a8775e30/Untitled%206.png)

C=1nF, R=+∞, Circuits du premier ordre

![Untitled](7%204%20674c023a6c0648f0addb10a3a8775e30/Untitled%207.png)

C=1nF, R=+∞, Circuits du deuxième ordre

![Untitled](7%204%20674c023a6c0648f0addb10a3a8775e30/Untitled%208.png)

C=1nF, R=+∞, Circuits du troisième ordre

![Untitled](7%204%20674c023a6c0648f0addb10a3a8775e30/Untitled%209.png)

C=0.15nF, R=24kΩ, Circuits du premier ordre

![Untitled](7%204%20674c023a6c0648f0addb10a3a8775e30/Untitled%2010.png)

C=0.15nF, R=24kΩ, Circuits du deuxième ordre

![Untitled](7%204%20674c023a6c0648f0addb10a3a8775e30/Untitled%2011.png)

C=0.15nF, R=24kΩ, Circuits du troisième ordre

![Untitled](7%204%20674c023a6c0648f0addb10a3a8775e30/Untitled%2012.png)

C=0.15nF, R=240kΩ, Circuits du premier ordre

![Untitled](7%204%20674c023a6c0648f0addb10a3a8775e30/Untitled%2013.png)

C=0.15nF, R=240kΩ, Circuits du deuxième ordre

![Untitled](7%204%20674c023a6c0648f0addb10a3a8775e30/Untitled%2014.png)

C=0.15nF, R=240kΩ, Circuits du troisième ordre

![Untitled](7%204%20674c023a6c0648f0addb10a3a8775e30/Untitled%2015.png)

C=0.15nF, R=+∞, Circuits du premier ordre

![Untitled](7%204%20674c023a6c0648f0addb10a3a8775e30/Untitled%2016.png)

C=0.15nF, R=+∞, Circuits du deuxième ordre

![Untitled](7%204%20674c023a6c0648f0addb10a3a8775e30/Untitled%2017.png)

C=0.15nF, R=+∞, Circuits du troisième ordre

![Untitled](7%204%20674c023a6c0648f0addb10a3a8775e30/Untitled%2018.png)

---

**Quelques réflexions:**

1. Le front montant gauche d'une onde carrée : plus facile à produire
Maintien à niveau élevé pendant un certain temps : difficile de maintenir à niveau élevé pendant un certain temps car le signal qui passe est à basse fréquence et le condensateur perd plus d'électrons avant d'être rechargé.
Le front descendant droit d'une onde carrée : le taux de chute peut être contrôlé en ajustant l'ordre du filtre et l'effet global est meilleur que le front montant d'un filtre passe-haut.
2. En augmentant l'ordre du filtre, celui-ci devient plus sensible, mais globalement, une plus grande partie de l'énergie du signal est filtrée, ce qui se traduit par l'observation de valeurs plus petites.
3. La diminution de la capacité du montage de détection de l'enveloppe ou l'augmentation de la résistance du montage de détection de l'enveloppe augmentera la valeur d'observation.

**Question:**

Actuellement, il y a des avantages et des inconvénients à chacun des filtres RC passe-bas ou passe-haut, mais aucun ne change assez rapidement autour de la fréquence de coupure.
La prochaine étape consistera peut-être à envisager d'autres structures de filtres ou des filtres actifs.
****