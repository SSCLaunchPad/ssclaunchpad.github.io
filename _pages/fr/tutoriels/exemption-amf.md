---
title: Configuration de l'authentification multifacteur (exempté)
altLangPrefix: mfa-exemption
description: Configuration de l'authentification multifacteur (exempté)
tags: [amf, securite]
---

### Introduction
<div class="alert alert-warning">
    <p>Cette page est écrite <b>seulement</b> pour les gens ayant été accordés par une exemption de notre politique normal d'authentification multifacteur pour des raisons approuvées.</p>
</div>

<div class="alert alert-warning">
    <p>L'option <b>SMS</b> est techniquement disponible en ce moment si vous avez eu une exemption d'AMF, cependant, cette option ne sera plus valide bientôt étant donné qu'elle n'est pas sécuritaire. Nous recommandons donc de suivre les instructions de cette page pour configurer un AMF par <em>TOTP</em></p>
</div>

Cette page contient les instructions qui vont vous aider à configurer une authentification multifacteur (AMF) à *TOTP* ([Mot de passe à usage unique basé sur le temps](https://fr.wikipedia.org/wiki/Mot_de_passe_%C3%A0_usage_unique_bas%C3%A9_sur_le_temps)), et ce, lorsqu'une exemption vous a été donnée afin de pouvoir utiliser une méthode moins sécurisée que l'AMF par notification (*push*). Cette exemption est donnée lors de circonstances spéciales et est dictée par notre équipe. Nous vous demandons de contacter notre équipe avant de suivre ces instructions.

#### Instructions

- Lors de la première connexion à notre environnement (si vous êtes exempté de la méthode d'AMF la plus sécurisée), on va vous demander de configurer votre AMF avec plusieurs options affichées à l'écran. Sélectionné l'option «Microsoft Authenticator»  
![](/assets/images/fr_sign_in_methods.png)

- Ensuite, cliqué sur l'option «Je souhaite utiliser une autre application d'authentification». Cette option n'est vraiment que disponible si vous êtes sur la liste d'exemption.  
![](/assets/images/fr_use_different_app.png)

- Suivez les instructions pour configurer un nouveau compte dans votre application d'authentification (il est possible d'utiliser n'importe quelle application d'authentification TOTP comme Google Authenticator par exemple).

- Numérisez le code QR donné à l'aide de votre application d'authentification.  
![](/assets/images/fr_auth_qr_code.png)


- Entrer le code à 6 chiffres donné par votre application.

- Votre application est maintenant configurée et devait maintenant fonctionner.

#### Applications TOTP recommandés

- Google authenticator 
- Proton authenticator
- LastPass Authenticator