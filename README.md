# HOLDI Landing Page 

This is the landing page for Holdi, a new startup that aims to automate investments for individuals. Created for Nicolas.

## Installation
To set up this project locally, follow these steps:
```bash
git clone https://github.com/alexkocev.github.io/holdi_landing_page.git
cd holdi
``` 

## Usage
Visit the URL [https://alexkocev.github.io/holdi_landing_page/](https://alexkocev.github.io/holdi_landing_page/)



### Additional Notes
**How to convert from Nice Page to raw code hosted in Github?**: 
 - Create a new folder Contact as: Contact/index.html & Contact/Contact.css

 - Delete *root/index.html*

 - Replace *Accueil.html* and *Accueil.cdd* by *index.html* & *index.css* as this is the homepage

 - Remove in *Contact/index.html* & *index.html*
		 - `<section class="u-backlink u-clearfix u-grey-80">...</section>`

    
- Update path in Contact/index.html with:
        - `href="../">Accueil</a>**`
        - `href="/Contact/">Contact</a>`
        - `href="../images/Holdilogowhitetrans.png"`
        - `src="../images/holdi5.png"`
        - `src="../jquery.js"`
        - `src="../nicepage.js"`
        - `href="../nicepage.css"`

- Update path in index.html with: 
        - `href="./">Accueil</a>`
        - `src="./images/holdi5.png"`
        - `href="/Contact/">Contact</a>`
        - `href="index.css"`

- Update path in index.css with: 
        - `src="./images/holdi5.png"`

- We use Formspree in Contact page. Replace:
```
<form action="https://forms.nicepagesrv.com/v2/form/process" class="u-clearfix u-form-spacing-19 u-form-vertical u-inner-form" source="email" name="form" style="padding: 19px;">
    <div class="u-form-email u-form-group">
      <label for="email-db6f" class="u-custom-font u-heading-font u-label">Email</label>
      <input type="email" placeholder="Entrez votre addresse email" id="email-db6f" name="email" class="u-border-none u-custom-color-4 u-custom-font u-heading-font u-input u-input-rectangle u-radius-10" required="">
    </div>
    <div class="u-form-group u-form-name u-form-partition-factor-2 u-form-group-2">
      <label for="name-961f" class="u-custom-font u-heading-font u-label">Prénom</label>
      <input type="text" placeholder="Entrez votre prénom" id="name-961f" name="name-1" class="u-border-none u-custom-color-4 u-custom-font u-heading-font u-input u-input-rectangle u-radius-10" required="">
    </div>
    <div class="u-form-group u-form-name u-form-partition-factor-2 u-form-group-3">
      <label for="name-961f" class="u-custom-font u-heading-font u-label">Nom</label>
      <input type="text" placeholder="Entrez votre nom" id="name-961f" name="name-2" class="u-border-none u-custom-color-4 u-custom-font u-heading-font u-input u-input-rectangle u-radius-10" required="">
    </div>
    <div class="u-form-group u-form-message">
      <label for="message-db6f" class="u-custom-font u-heading-font u-label">Message</label>
      <textarea placeholder="Êtes vous intéressé par notre offre? Souhaitez vous en savoir plus? Dites nous ce que vous voulez." rows="4" cols="50" id="message-db6f" name="message" class="u-border-none u-custom-color-4 u-custom-font u-heading-font u-input u-input-rectangle u-radius-10" required=""></textarea>
    </div>
    <div class="u-align-right u-form-group u-form-submit">
      <a href="#" class="u-border-none u-btn u-btn-round u-btn-submit u-button-style u-custom-color-3 u-custom-font u-heading-font u-radius-20 u-btn-1">Envoyer</a>
      <input type="submit" value="submit" class="u-form-control-hidden">
    </div>
```
with
```
<form action="https://formspree.io/f/..." method="POST" class="u-clearfix u-form-spacing-19 u-form-vertical u-inner-form" style="padding: 19px;">
  <div class="u-form-group">
    <label for="first-name" class="u-custom-font u-heading-font u-label">Prénom</label>
    <input type="text" id="first-name" name="first_name" placeholder="Entrez votre prénom" class="u-border-none u-custom-color-4 u-custom-font u-heading-font u-input u-input-rectangle u-radius-10" required>
  </div>
  <div class="u-form-group">
    <label for="last-name" class="u-custom-font u-heading-font u-label">Nom</label>
    <input type="text" id="last-name" name="last_name" placeholder="Entrez votre nom" class="u-border-none u-custom-color-4 u-custom-font u-heading-font u-input u-input-rectangle u-radius-10" required>
  </div>
  <div class="u-form-email u-form-group">
    <label for="email" class="u-custom-font u-heading-font u-label">Email</label>
    <input type="email" id="email" name="email" placeholder="Entrez votre addresse email" class="u-border-none u-custom-color-4 u-custom-font u-heading-font u-input u-input-rectangle u-radius-10" required>
  </div>
  <div class="u-form-group u-form-message">
    <label for="message" class="u-custom-font u-heading-font u-label">Message</label>
    <textarea id="message" name="message" placeholder="Êtes vous intéressé par notre offre? Souhaitez vous en savoir plus? Dites nous tout!" class="u-border-none u-custom-color-4 u-custom-font u-heading-font u-input u-input-rectangle u-radius-10" required></textarea>
  </div>
  <div class="u-align-right u-form-group u-form-submit">
    <input type="submit" value="Envoyer" class="u-border-none u-btn u-btn-round u-button-style u-custom-color-3 u-custom-font u-heading-font u-radius-20">
  </div>
```
    

 - Google Analytics to add in the headers for *index.html* and *Contact/index.hmtl*
    
```
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-..."></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-...');
</script>
```
