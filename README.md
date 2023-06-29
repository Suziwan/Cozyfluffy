# Cozy & Fluffy

## Description <img src=/app/assets/images/cozy.png width="200" align="right" />
Ce projet de site web est la vitrine d'un salon de thé associatif sur le concept de bar à chats, l'association à but non lucratif "Cozy & Fluffy" accueille donc des chats de manière permanente ou temporaire et facilite leur adoption. Les fonds du salon de thé servent à faire fonctionner l'association.  

Il ne s'agit pas d'un salon de thé physique ou d'une association réelle, mais d'une idée de site web pour le projet final de la formation THP Fullstack du groupe Cozy & Fluffy.  
Lien du site en production : https://cozyfluffy.herokuapp.com (hors ligne)

## Cahier des charges
- Executive summary, disponible sur [Google Docs](https://docs.google.com/document/d/1DrETqztTcQTJiFipLb5W6aw6aajQehMRc0twlfnxpyc/edit#heading=h.lekq4on0km5s)
- Users stories, disponible sur [Trello](https://trello.com/b/3cWWWov9/cozy-fluffy)
- Design du site, disponible sur [Figma](https://www.figma.com/file/yt0mUXTpcsOyUIc003yAZc/Untitled?node-id=0-1&t=2N2gOae54vuPXuQP-0)
- Parcours utilisateur, disponible sur [Lucid](https://lucid.app/lucidchart/07ca552f-653f-4de0-93ee-92b8eed5fcba/edit?viewport_loc=-35%2C34%2C1707%2C779%2C0_0&invitationId=inv_f69a61cd-d4fb-4853-abf5-6cd8efadf594)

## Membres du groupe
- Lisa Daudibon ([@LisaDaudibon](https://github.com/LisaDaudibon))
- Karine Da Silva ([@KarineDHoshi](https://github.com/KarineDHoshi))
- Chandara Loek ([@Daralafada](https://github.com/Daralafada))
- Suzanne Christé ([@Suziwan](https://github.com/Suziwan))

## Versions, gems et API utilisées
Ruby 3.0.0, Rails 7.0.4.2, PostgreSQL 1.1.  
Gems importantes : [Stripe](https://github.com/stripe/stripe-ruby), [Simple Calendar](https://github.com/excid3/simple_calendar), [Devise](https://github.com/heartcombo/devise), [Dotenv](https://github.com/bkeepers/dotenv), [I18n](https://github.com/ruby-i18n/i18n).  
Gems de tests : [Rspec-rails](https://github.com/rspec/rspec-rails), [FactoryBot Rails](https://github.com/thoughtbot/factory_bot_rails), [NyanCatFormatter](https://github.com/mattsears/nyan-cat-formatter).  
API intégrées : [Stripe](https://stripe.com/docs/api), [Sendgrid](https://sendgrid.com/solutions/email-api/), [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/api/).  
Hébergement : Heroku.

## Lancement du programme en local
Télécharger le dossier GitHub en local ou le cloner, puis vérifier les versions utilisées.  
Dans le terminal, exécuter les lignes suivantes :
- `bundle install` pour installer les versions et gems mentionnées.
- `rails assets:precompile` pour compiler les fichiers CSS et JS utilisés.
- `rails db:create db:migrate db:seed` pour créer et remplir la base de données.
- `rails s` pour lancer le serveur et visualiser le site sur http://localhost:3000.  

NB : Les fonctionnalités utilisant des clés API comme les mails, paiements et affichage de la carte peuvent ne pas fonctionner.

## Tester le programme en local
Pour utiliser les gems de tests, exécuter les lignes suivantes dans le terminal :
- `rspec` pour lancer les 100 tests préparés.
- `rspec spec/requests/users_spec.rb` pour lancer les tests sur un fichier spécifique.
- `rspec --format NyanCatFormatter` pour lancer les tests en utilisant la gem NyanCatFormatter.

## Diagramme ER base de données
Ci-dessous un diagramme entité-relation de la base de données utilisée :  

<img src=/app/assets/images/database_cozyfluffy.png width="700">

## Home page overview

<object data="https://github.com/Suziwan/Cozyfluffy/blob/development/documents/CozyFluffy_Home.pdf" type="application/pdf" width="700px" height="700px">
    <embed src="https://github.com/Suziwan/Cozyfluffy/blob/development/documents/CozyFluffy_Home.pdf">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="https://github.com/Suziwan/Cozyfluffy/blob/development/documents/CozyFluffy_Home.pdf">Download PDF</a>.</p>
    </embed>
</object>