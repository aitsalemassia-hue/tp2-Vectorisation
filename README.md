Questions :
Partie 5 — Représentation Bag of Words:

1. Que représente chaque colonne de la matrice ?
  Chaque colonne correspond à un mot unique du vocabulaire extrait du corpus. 

2. Quelles sont les limites du modèle Bag of Words ?
  -Il ignore la position des mots.
  -Il n'y a pas de pondération entre les mots fréquents et les mots rares.
  -Les mots très fréquents dominent souvent la représentation.

3. Que perd-on en supprimant l'ordre des mots ?
  On perd le sens construit par la structure de la phrase.

Partie 6 — Représentation TF-IDF

1. Quelle est la différence principale entre BoW et TF-IDF ?
   Le TF-IDF donne de l'importance aux mots rares, alors que le BoW ne fait pas la différence
   entre les mots rares et les mots fréquents dans le corpus.
2. Pourquoi les mots très fréquents ont-ils souvent un poids faible ?
   Car l'IDF = log(N / DF(t)) devient très petit quand le mot apparaît dans beaucoup de documents (DF proche de N).
   Si DF = N, alors log(N/N) = log(1) = 0, donc son poids est réduit.
