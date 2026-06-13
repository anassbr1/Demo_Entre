
> ⚠️ L’application utilisateur **ne nécessite pas** `admin.html` pour fonctionner. Elle utilise des valeurs par défaut si aucune décision forcée n’est présente.

---

## 🚀 Installation et utilisation

1. **Téléchargez** le fichier `user.html`.
2. **Ouvrez‑le** dans n’importe quel navigateur moderne (Chrome, Edge, Firefox, Safari).
3. **Autorisez l’accès à la caméra** si vous souhaitez utiliser le scan en direct.
4. **Connectez‑vous** avec le profil citoyen (un simple clic).
5. **Scannez** un médicament :
   - Activez la caméra et prenez une photo, ou
   - Importez une image depuis votre galerie.
6. **Observez le résultat** : authentique ✅ ou alerte 🚨, avec détails du lot, fabricant, marqueurs de sécurité.
7. **Consultez l’historique** et votre profil.

---

## ⚙️ Personnalisation

### 📦 Base de données par défaut
Par défaut, l’application utilise un médicament **Doliprane 1000 mg** comme authentique. Vous pouvez modifier la constante `DEFAULT_DECISION` dans le code pour changer les valeurs par défaut.

### 🧠 Forcer une décision (si vous utilisez `admin.html`)
L’application lit la clé `admin_decision` dans `localStorage`. Un administrateur peut donc y stocker un objet JSON du type :

```json
{
  "verdict": true,
  "nom": "Doliprane 1000 mg",
  "lot": "23B12",
  "fabricant": "Sanofi",
  "exp": "2028-12",
  "pays": "France",
  "score": 99.8,
  "message": "...",
  "marqueurs": ["Hologramme détecté", "Code QR valide"]
}
Si cette clé existe, son contenu est utilisé à la place de la logique de détection normale.

📸 Captures d’écran
(Ajoutez ici quelques images de l’application si vous le souhaitez)

🤝 Contribution
Les contributions sont les bienvenues !
Si vous souhaitez améliorer la logique de détection, l’interface ou corriger des bugs, n’hésitez pas à ouvrir une issue ou une pull request.

📄 Licence
Distribué sous licence MIT. Voir le fichier LICENSE pour plus d’informations.

📬 Contact
Projet réalisé par Anass Bouras et son équipe pour la lutte contre la contrefaçon pharmaceutique.
Pour toute question : anass.bouras2018@gmail.com

PharmaScan AI – Protéger la santé par la technologie.

---

Copiez ce contenu dans un fichier `README.md` et placez‑le dans le même dossier que `user.html`. Si vous hébergez également `admin.html`, vous pouvez mentionner le lien vers son README dédié.