# SMB215

Le projet est composé de 5 types d’utilisateurs : le client, gestionnaire d’inventaire, gestionnaire de l'entrepôt, Gestionnaire du chauffeur et le chauffeur.
1)	Créer un bien 

a)	Le gestionnaire d'inventaire est responsable de la création d'éléments dans le système. Chaque article a un type, marque, code, catégorie, nom, quantité, code a barre, date de fabrication, date d’expiration, cout, prix, unité de mesure, description et les locations {Corridor, étagère, taille, nom de l’entrepôt et la quantité}.

2)	Les transferts

a)	Le gestionnaire d'inventaire, le gestionnaire d’entrepôt effectuent un transfert interne (entre 2 entrepôts) et le client faire une commande afin qu’il créer un transfert externe (entre client et entrepôt) en utilisant les commandes d'expédition. Chaque commande d'expédition contient la source et la destination de l’entrepôt ou client, la date et la liste des produits. Une fois la commande envoyé, Gestionnaire du chauffeur doit organiser l'horaire de l'expédition en utilisant le picking waves (décidez les transactions en manière prioritaire).
	
3)	Réceptionner un bien et le placer dans un lieu 

a)	Lorsque les produits sont reçus dans l'entrepôt, le gestionnaire d'entrepôt doit faire un scan de code à barres pour savoir leurs places dans l’entrepôt afin de les remplir. 
b)	Le gestionnaire d'entrepôt doit entrer la quantité reçue, en plus il pourra ajouter une nouvelle location. 
c)	Si le produit reçu n'existe pas, ils doivent retourner a (1. Créer un bien) donc envoyer un mail pour gestionnaire d’inventaire afin de créer le produit.



4)	Promotion sur un bien (entrepôt virtuelle)

a)	Choisissez la description de l'élément du nouveau produit (coordinateur) 
b)	Assigne un nouveau code à barres (coordinateur) 
c)	Envoie le coût, prix et la description des codes-barres à l’inventaire afin de publier le produit sur le système 
d)	Exécutez un bon de commerce pour transférer de l'entrepôt principal à l'entrepôt de promotion afin d'avoir les articles prêts dans l'entrepôt de promotion pour la manipulation. 
e)	Après avoir fini la manipulation, le coordonnateur doit obtenir le nombre exact des offres effectuées (certaines offres expirées, endommagées, perdues) 
f)	Assembler le composant de l’offre (1 ou plus) en un produit final 
g)	L'inventaire doit afficher le produit sur le système avec ses quantités. 
h)	Le coordinateur doit envoyer un bon de transfert à l'entrepôt pour transférer les quantités de l'entrepôt promotion à l'entrepôt principal (en main). 
i)	Mettez à jour un nouveau bon de commerce contenant le produit afin de pouvoir le vendre.



5)	Produits endommagés (entrepôt virtuel) 

a)	L'entrepôt doit faire un bon de transfert de l'entrepôt principal à l'entrepôt endommagé en déduisant la quantité.



6)	Déplacer un bien 

a)	Si vous devez déplacer un produit de l'entrepôt principal vers n'importe quel autre emplacement ou entrepôt, le gestionnaire de l'entrepôt doit recevoir (bon de commande BDC par courrier électronique) du coordinateur, en demandant le mouvement du produit
b)	Le gestionnaire du chauffeur choisis les chauffeurs en manière optimale.

7)	Vendre un bien 

a)	Après avoir reçu un ordre achat du client, ou remplir un BDC (bon de commerce). Il sera envoyé à l'entrepôt pour préparer la commande. Le BDC contient le code, la description de l'article, le prix et la quantité gratuite si disponible.
b)	Le travailleur de l'entrepôt doit entrer le code de l'élément dans l'application afin de montrer les informations sur le produit spécifique (la rangée, l'étagère, la direction). 
c)	Lorsque le travailleur de l'entrepôt trouve que le produit sur l'étagère doit analyser le code à barres et entrer la quantité déduite du stock. Et qu'il prépare les articles à envoyer au client au lendemain.



8)	Bien consommable fin de vie

a)	Le système doit mettre en évidence le produit dans le tableau avant la date de péremption dans un délai précis.
