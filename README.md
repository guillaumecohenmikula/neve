# Neve

Outil de gestion B2B pour de la revente à la commande, sans stock :

- **Modèles** : coloris, paliers de prix d'achat fournisseur et de prix de gros, prix de vente conseillé.
- **Devis** aux revendeurs : lignes modèle × coloris × pointures, prix de gros calculé selon les paliers.
- **Commandes fournisseur** : regroupement des devis signés, coût d'achat et marge brute.

Front statique (HTML/JS, un seul fichier) branché sur Supabase (authentification + Postgres).
La clé Supabase visible dans le code est la clé publique (publishable), prévue pour vivre dans le front :
les données sont protégées par la sécurité au niveau des lignes (RLS), chaque compte ne voit que les siennes.

Ce dépôt ne contient que la version publiée de l'app, servie par GitHub Pages.
