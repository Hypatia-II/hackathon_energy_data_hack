# Energy data hack
## Challenge 1 : Interception des ondes radios sur les capteurs d’énergies

<p align="center">

<a >
    <img src='./images/logo_hackaton.png'  width="400"/>
</a>

</p>

Hacker le login et le mdp sur une interception d'ondes radios


## Installation

Utiliser un 'venv' ou un environnement 'conda', puis récupérer les versions :
```
pip install -r requirements.txt
```

## Entrainement des modèles

- Utilisation de MLP, GRU et Random Forest pour la classification multi-classe (42 classes)

| Accuracy | F1 score |
|---| --- |
| ![](/images/acc.png) | ![](/images/f1_scores.png) |


- Utilisation de MLP et GRU pour données regroupées en groupe de trames : 1, 5, 10, 25, 100 et 200

| MLP | GRU |
|---| --- |
| ![](/images/acc_without_noise_mlp.png) | ![](/images/acc_without_noise_gru.png) |


- Utilisation de MLP et GRU pour données regroupées en groupe de trames avec ajout de bruit sur les données d'entrainement

| MLP | GRU |
|---| --- |
| ![](/images/acc_noise_mlp.png) | ![](/images/acc_noise_gru.png) |
