# duchadeau_project
Brainhack-school 2024 repository of Romain DUCHADEAU

## Who am I ?
<a href="https://github.com/romainDCHD ">
   <img src="https://avatars.githubusercontent.com/romainDCHD?v=4?s=100" width="100px;" alt=""/>
   <br /><sub><b>Romain DUCHADEAU</b></sub>
</a>

I am a microelectronics engineering student at Polytechnique Montréal who wishes to specialize in biomedical


# Dataset Description

Ce dataset comprend des enregistrements simultanés d'EEG et de signaux BOLD de 33 participants en bonne santé, collectés à l'Université de l'État de Pennsylvanie avec leur consentement éclairé.

## Contenu du Dataset

### Participants
- 33 participants en bonne santé.

### Sessions d'enregistrement
- Sessions anatomiques pour l'imagerie structurelle.
- Deux sessions de repos de 10 minutes chacune.
- Plusieurs sessions de sommeil de 15 minutes chacune.
- La première session de repos a été réalisée avant une tâche d'adaptation visuo-motrice (Albouy et al, Journal of Sleep Research, 2013) et la deuxième session de repos après cette tâche.

### Données de stades de sommeil
- Les stades de sommeil pour ces 33 sujets sont organisés dans le dossier 'sourcedata'.
- Chaque fichier TSV contient les stades de sommeil pour chaque intervalle de 30 secondes à travers différentes sessions pour chaque sujet.
- Les notations incluent : "w" pour l'éveil, "1" pour NREM1, "2" pour NREM2, "3" pour NREM3, "uncertain" pour les périodes incertaines, et "unscorable" pour les périodes avec des artefacts trop importants pour être scorées de manière fiable.

### Imagerie par résonance magnétique (IRM)
- Données collectées sur un scanner Prisma Siemens Fit 3 Tesla utilisant une bobine de réception 20 canaux Siemens.
- Images anatomiques acquises avec une séquence MPRAGE (TR : 2300 ms, TE : 2.28 ms, résolution spatiale isotropique de 1 mm, FOV : 256 mm, angle de bascule : 8 degrés, taille de la matrice : 256×256×192, facteur d'accélération : 2).
- Données fMRI BOLD acquises avec une séquence EPI (TR : 2100 ms, TE : 25 ms, épaisseur de coupe : 4 mm, 35 coupes, FOV : 240 mm, résolution in-plane : 3 mm×3 mm).

### Données EEG
- Collectées avec un système EEG 32 canaux compatible IRM de Brain Products, Allemagne.
- Électrodes placées selon le système international 10-20.
- Enregistrements de l'activité oculaire (EOG) et du signal cardiaque (ECG).
- Données EEG collectées à une fréquence d'échantillonnage de 5000 Hz avec un filtre passe-bande de 0-250 Hz.
- R128 dans les signaux EEG correspond au déclencheur de volume BOLD fMRI.
- Marqueurs S1 dans l'EEG pendant les sessions de sommeil indiquant l'état d'éveil des participants. Les marqueurs S2 et S3 représentent l'absence de pression de bouton et peuvent être ignorés.

## Application du Dataset

Ce dataset est idéal pour développer un algorithme permettant de détecter si un participant est en état de sommeil ou d'éveil en utilisant les enregistrements EEG et fMRI. Vous pouvez utiliser les stades de sommeil notés pour entraîner un modèle de machine learning capable de distinguer les états de sommeil et d'éveil.

Pour plus d'informations ou des questions sur ce dataset, veuillez consulter les articles mentionnés dans la section "References and Links" du dataset ou contacter le Dr. Yameng Gu (ymgu95@gmail.com).


# TODO

1. Sous quelle forme (image, info) mettre les datas pour le donner au ML
2. Comment traiter les datas (epoch?, mask?, altas?, utilisation de T1?)
3. Comment ils s'y sont pris pour savoir si c'est éveillé ou pas???
4. Quelle différence entre la feature extraction `fmri_data = fmri_img.get_fdata` et avec les masker comme celui ci :
```
masker = NiftiLabelsMasker(labels_img=atlas_filename, 
                           standardize=True, 
                           memory='nilearn_cache', 
                           verbose=1)
```


# Autre ressources :
- [Preprocessing workflow](https://peerherholz.github.io/workshop_weizmann/nipype/notebooks/handson_preprocessing.html)
- [Lien d'un projet similaire de la brainhack-school](https://school-brainhack.github.io/project/fmri-sleep-deprivation/)
- [Data preprocessing git cool avec docker](https://fmriprep.org/en/stable/) 
- [Etapes preprocessing](https://carpentries-incubator.github.io/SDC-BIDS-fMRI/instructor/aio.html)
- [nipype](https://nipype.readthedocs.io/en/latest/)