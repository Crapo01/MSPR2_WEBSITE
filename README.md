
# DEPLOIEMENT D'UNE NOUVELLE INSTANCE REACT VITE:

Cloner le repo.

Aller à la racine du site cd MSPRFRONT

  npm install

va installer toutes les dependances:

"dependencies": {

    "react": "^18.2.0", 

    "bootstrap": "^5.3.3",

    "leaflet": "^1.9.4",

    "leaflet-routing-machine": "^3.2.12",

    "react-bootstrap": "^2.10.3",

    "react-dom": "^18.3.1",

    "react-html-parser": "^2.0.2",

    "react-leaflet": "^4.2.1",

    "react-router-dom": "^6.23.1"
  },

  Configurer les Variables d’Environnement

📌 Créer un fichier .env dans le dossier racine et ajouter les variables nécessaires :

Ajoute tes variables d’environnement :

    VITE_SITE_KEY = 

📌 Mettre à jour scr/config/config.js et ajouter l’URL de base:

    //export const BASE_URL="http://localhost:8080";
    export const BASE_URL="https://msprback-cms-reworked.onrender.com";




  # lancement de l'app+serveur applicatif

  Aller à la racine du site et lancer dans la console:  
  
    npm run dev 

  # BUILD de l'app pour deploiement WEB

  Aller à la racine du site et lancer dans la console:

    npm run build

  le build est dans le dossier dist

  # deploiement sur serveur WEB

  transferer l'ensemble du dossier dist via  filezilla dans le dossier HTDOCS du serveur web

  # MSPR2 development steps

  ## Connect to API

  no changes in code:

  updated end points:

  API concert end point:  
  api/concerts/all"

  API actus end point:  
  api/informations/all

  API pointeur end point:  
  api/pointeurs/all

## Security

added signup/login/logout

source:  
[react-jwt-auth](https://www.bezkoder.com/react-jwt-auth/)

users are registered with ROLE_NONE role automatically.

## reCAPTCHA implementation

[react recaptcha](https://shejanmahamud.medium.com/implement-google-recaptcha-in-react-app-a9b8e3dc26ed)  
[useref in class components](https://stackoverflow.com/questions/62499061/how-to-use-react-useref-in-class-component) 



### backend validation

[springboot recaptcha validation](https://www.pixeltrice.com/recaptcha-validation-in-registration-form-using-spring-boot-application/)

endpoint api/auth/verify

## PUSH NOTIFICATIONS

    
resource:

[send-push-from-spring-boot-backend-to-react](https://hpcodes.medium.com/send-messages-from-spring-boot-backend-to-reactjs-app-using-websocket-4120f6979c9b)

https://www.npmjs.com/package/react-stomp-hooks

added publish message TODO MESSAGING QUEUE LOGIC

https://www.npmjs.com/package/react-toastify

  npm install --save react-toastify

