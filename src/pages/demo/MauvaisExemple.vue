<template>
  <Layout>
    <div class="dg-content fr-px-2w fr-pt-4w">

      <h1>Trouve les erreurs !</h1>
      <p>Cette page a été créée avec des erreurs - volontaires, c’est un exercice - de design et d’accessibilité. Sauras-tu les retrouver ? <br>(pour t’aider, tu peux utiliser le <a href="/outils/diagnostic-flash/">diagnostic flash</a>)</p>

      <section class="fixed-width">
        <h3>Tout savoir sur la bicyclette</h3>
        <p>Une bicyclette, ou un vélo (abréviation du mot vélocipède), est un véhicule terrestre à propulsion humaine entrant dans la catégorie des cycles et composé de deux roues alignées, qui lui donnent son nom. La force motrice est fournie par son conducteur (appelé « cycliste »), en position le plus souvent assise, par l’intermédiaire de deux pédales entraînant la roue arrière par une chaîne à rouleaux.</p>
        <p>La roue avant est directrice et assure l’équilibre. Son orientation est commandée par un guidon. Le cycliste a souvent les deux mains en contact avec le guidon afin de contrôler la trajectoire, le freinage ainsi que le passage des vitesses.</p>
        <p>La <a tabindex="1" style="border-bottom: none" class="lien" href="https://fr.wikipedia.org/wiki/Bicyclette" target="blank" >bicyclette</a> est l’un des principaux moyens de transport dans de nombreuses parties du monde. Son efficacité énergétique est particulièrement élevée. Sa pratique, le cyclisme, constitue à la fois un usage quotidien de transport, un loisir populaire et un sport.</p>
        <p><!-- balise utilisée à des fins de  présentation --></p>
        <p><!-- balise utilisée à des fins de  présentation --></p>
      </section>
      <img src="/assets/images/bike.png" style="width:100%"  alt="L’anatomie d’une bicyclette"  />
      <section class="fr-grid-row fr-grid-row--center">
        <div class="fr-col-12">
          <h3>Tout savoir sur le RGAA</h3>
          <div class="fr-content-media__img">
            <img src="/assets/images/seguRgaaNuit.jpg" class="fr-responsive-img" alt="" style="width:100%" />
          </div>
        <p>Si vraiment l’accessibilité numérique vous intéresse, vous pouvez tout à fait télécharger le rgaa <a style="border-bottom: none" tabindex="3" class="lien" href="https://www.numerique.gouv.fr/uploads/rgaa/RGAA-v4.1.pdf">ici</a> ou le voir en ligne <a style="border-bottom: none" tabindex="2" class="lien" href="https://www.numerique.gouv.fr/publications/rgaa-accessibilite/">là</a>.</p>
        </div>
      </section>
      <section class="fr-grid-row fr-grid-row--center">
        <div class="fr-col-8">
          <form action="#" method="post" rel="noreferrer noopener">
            <fieldset><legend><h4>Mieux se connaître</h4></legend>
            <p class="indicates-required">Les champs en jaune sont obligatoires</p>

            <div class="form-group fr-mt-4w">
              <label class="fr-label">Votre adresse électronique</label>
              <input tabindex="-1"class="fr-input jaune" type="text" id="mail" name="text-input-text" required >
            </div>

            <div class="form-group fr-mt-4w">
              <label class="fr-label" for="pseudo">Votre pseudo</label>
              <input class="fr-input" type="text" id="pseudo" name="text-input-text" >
            </div>

            <div class="form-group fr-mt-4w">
              <label class="fr-label" for="like">Vous aimez ...</label>
                <select name="" class="fr-input"  >
                  <option value="1">les fruits et les légumes</option>
                  <option value="2">les ballades à bicyclette</option>
                  <option value="3">les voyages à vélo</option>
                  <option value="4">faire la sieste</option>
                  <option value="5">rien de tout ça</option>
                </select>
            </div>


            <div class="form-group fr-mt-4w">
              <input class="fr-btn" type="submit" id="pseudo" name="valider" value="Valider" />
            </div>

            <p class="rgpd rgpd--small">
              Conformément à la règlementation, vous disposez d’un droit d’opposition et d’un droit à la limitation du traitement de données vous concernant, ainsi que d’un droit d’accès, de rectification, de portabilité et d’effacement de vos données. Vous pouvez exercer vos droits en nous écrivant à l’adresse électronique suivante : contact@design.numerique.gouv.fr.
            </p>
            </fieldset>
          </form>
        </div>
      </section>

      <p>Vous avez terminé ?<br>Combien d’erreurs avez-vous trouvé ?</p><p>Vous pouvez télécharger le <a href="/assets/doc/diagnostic-flash-exercice.ods" download>diagnostic flash complété et corrigé (fichier ods - 44 Ko)</a> et vous rendre sur une <a href="../bon-exemple/">page sans erreur</a>.</p>

    </div>
  </Layout>
</template>


<script>
  export default {
    metaInfo: {
      title: "Test",
      description: "Cette page web regroupe plusieurs mauvaises pratiques.",
      meta: [{
        name: "robots",
        content: "noindex"
      }],
    }
  }
</script>


<style scoped lang="scss">

  section.fixed-width {
    width: 36em;
    text-align: justify;
    margin: auto;

    a.lien {
      border-bottom: none;
      text-decoration: none;
    }
  }

  h3 {
    color: chartreuse;
  }

  .jaune {
    background-color: yellow;
  }

  .indicates-required {
    text-align: right;
  }

</style>

<!--

Les anomalies sont les suivantes :
* title non pertinent
* largeur fixe : scroll horizontal en mobile
* l'information ne doit pas passer que par la couleur : lien non souligné, input jaune
* hierarchie des titres
* libellé des liens non explicite (lien externe, fichier à télécharger)
* libellé du bouton non explicite : à quoi sert le formulaire ?
* contraste des h3
* alternative non pertinente
* label non lié au select
* balise p utilisée à des fins de présentation poir passer une ligne
-->
