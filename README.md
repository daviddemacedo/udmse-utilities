# udmse-utilities

Suivre le déploiement des scripts via : 
https://github.com/boostchicken-dev/udm-utilities/tree/master/on-boot-script

Attention, il y a un bug avec le service udm-boot.service : 
Suivre ce qui est indiqué ici : 
https://github.com/boostchicken-dev/udm-utilities/issues/316


Pour installer podman, générer le build :
https://github.com/boostchicken-dev/udm-utilities/actions/workflows/podman-udmse.yml

Puis récupérer l'archive zip et le déziper directement dans le / de l'udmse. 

Pour avoir un podman fonctionnel, copier les fichiers présents dans le répertoire /podman de ce dépot en suivant l'arborescence.

Attention, en cas de mise à jour du firmware, il se pourrait que les fichiers modifiés présent dans le répetoire /usr de l'udmse soit supprimés (https://www.reddit.com/r/Ubiquiti/comments/q7qk3m/udm_se_persisted_debian_packages_installation/?sort=new). Donc plus de binaire podman installé. 
Il faudra donc remettre le contenu de /usr de l'archive udmse-podman-install.zip.zip récupérée via le build udm-utilities.  
