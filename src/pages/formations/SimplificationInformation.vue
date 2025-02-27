<template>
  <Layout>

    <div class="dg-cover dg-cover--linear fr-mb-6w">
      <div class="dg-cover__container fr-mb-1w">
        <nav aria-label="Breadcrumb" class="fr-breadcrumb">
          <ol class="fr-breadcrumb__list">
            <li>
              <g-link to="/" class="fr-breadcrumb__link">Accueil</g-link>
            </li>
            <li>
              <g-link to="/formations/" class="fr-breadcrumb__link">Formations</g-link>
            </li>
            <li>
              <span aria-current="page">Formation Simplification de l'information aux usagers</span>
            </li>
          </ol>
        </nav>
        <h1 class="dg-cover__title">Formation Simplification de l'information aux usagers</h1>
        <p class="fr-text--lead">Pourquoi et comment employer un langage simple et clair pour nos services publics, en explorant les subtilités du fonctionnement de notre cerveau.</p>
      </div>
    </div>

    <div class="dg-content dg-content--xs fr-px-2w fr-mt-6w">
      <h2>Revivez la formation en vidéo</h2>
      <p>La formation a eu lieu en direct le jeudi 17 février. Vous pouvez la revivre <a href="https://www.youtube.com/watch?v=7scX1FO_FQM" target="_blank" title="sur notre chaîne YouTube - Nouvelle fenêtre">sur notre chaîne YouTube</a> avec transcription par vélotypie.</p>

      <h3>Objectifs</h3>
      <ul>
        <li>Proposer une information adaptée aux usagers</li>
        <li>Prendre en compte la façon dont l’information est traitée</li>
        <li>Connaître les principes de simplification</li>
        <li>Appliquer une méthodologie de simplification centrée usager</li>
      </ul>

      <h3>Public concerné</h3>
      <p>Agents de la fonction publique ou prestataires impliqués dans la conception des services numériques publics.</p>

      <h3>Programme</h3>
      <ol>
        <li>Enjeux de simplification de l’information</li>
        <li>Comment le cerveau traite l’information</li>
        <li>Principes de conception d’une information adaptée</li>
        <li>Méthodologie de simplification centrée usager</li>
        <li>Conclusion</li>
      </ol>

      <h3>Formatrice</h3>
      <div class="person">
        <g-image src="~/assets/images/team-photos/camille-rozier.jpg" width="120" alt="" class="person__photo"/>
        <p class="person__description">
          <strong class="person__name">Camille Rozier</strong><br>
          Cheffe de projet simplification et sciences comportementales à la Direction interministérielle de la transformation publique (DITP)
        </p>
      </div>

      <h3>Ressources</h3>
      <ul class="fr-mb-4w">
        <li><a href="https://www.modernisation.gouv.fr/outils-et-formations/simplifier-les-documents-administratifs" target="_blank" title="Simplifier les documents administratifs : 6 vidéos et 6 fiches pratiques - nouvelle fenêtre">Simplifier les documents administratifs : 6 vidéos et 6 fiches pratiques</a> (DITP)</li>
        <li><a href="https://www.modernisation.gouv.fr/files/2021-06/guide_pratique_vaincre_la_phobie_administrative_com_4(1).pdf" target="_blank" title="Guide pratique vaincre la phobie administrative grâce aux sciences comportementales - nouvelle fenêtre">Guide pratique vaincre la phobie administrative grâce aux sciences comportementales</a> (DITP)</li>
        <li><a href="https://cnnumerique.fr/votre-attention-sil-vous-plait-quels-leviers-face-leconomie-de-lattention" target="_blank" title="Votre attention, s’il vous plaît ! Quels leviers face à l’économie de l’attention ? - nouvelle fenêtre">Votre attention, s’il vous plaît ! Quels leviers face à l’économie de l’attention ?</a> (Conseil national du numérique)</li>
        <li><a href="https://www.rhone.gouv.fr/content/download/16040/91641/file/LARA-1.pdf" target="_blank" title="Lexique administratif : un langage clair ça simplifie la vie - nouvelle fenêtre">Lexique administratif : un langage clair ça simplifie la vie</a> (Comité d’Orientation pour la Simplification du Langage Administratif (COSLA), Dictionnaires Le Robert)</li>
        <li><a href="https://editions.flammarion.com/systeme-1-systeme-2/9782081211476" target="_blank" title="Système 1 / Système 2, Les deux vitesses de la pensée - nouvelle fenêtre">Système 1 / Système 2, Les deux vitesses de la pensée</a> (Daniel Kahneman - Flammarion) </li>
        <li><a href="https://www.simonandschuster.com/books/Simpler/Cass-R-Sunstein/9781476726601" target="_blank" title="Simpler, The Future of Government - nouvelle fenêtre">Simpler, The Future of Government</a> (Cass R. Sunstein - Simon & Schuster)</li>
      </ul>


      <p>C’est important, c’est gratuit, c’est ludique, c’est opérationnel et, franchement, c’est bien fait donc : venez !</p>
      <p>N'oubliez pas, nous proposons d’autres formations à (re)visionner : <g-link to="/formations/design/">design</g-link>, <g-link to="/formations/accessibilite/">accessibilité</g-link>, <g-link to="/formations/recherche-utilisateur/">recherche utilisateur</g-link> et <g-link to="/formations/ecoconception/">écoconception</g-link>.</p>

      <!-- <h2>Inscription</h2>
      <p>Pour que nous puissions vous communiquer d'éventuelles précisions et que nous sachions qui se trouvera de l'autre côté de l'écran, vous pouvez nous envoyer ce formulaire.</p>
      <p><small>Tous les champs du formulaire sont obligatoires.</small></p>
      <form class="form" v-on:submit.prevent="addParticipant">
        <div class="fr-input-group">
          <label class="fr-label" for="email">Votre adresse e-mail<span class="fr-hint-text">L’adresse e-mail doit être au format prenom@mail.fr</span></label>
          <input class="fr-input" type="email" id="email" v-model="form.email" required>
        </div>
        <div class="fr-input-group">
          <label class="fr-label" for="organisme">Votre organisme</label>
          <input class="fr-input" type="text" id="organisme" v-model="form.organisme" required>
        </div>
        <p><small>Les données recueillies sur ce formulaire sont traitées par les équipes de la DINUM. Elles nous permettent de vous informer via e-mail des nouvelles liées à cet événement.</small></p>
        <p><small>Conformément à la règlementation, vous disposez d’un droit d’opposition et d’un droit à la limitation du traitement de données vous concernant, ainsi que d’un droit d’accès, de rectification, de portabilité et d’effacement de vos données. Vous pouvez exercer vos droits en nous écrivant à contact@design.numerique.gouv.fr.</small></p>
        <button class="fr-btn" id="submit" type="submit">S'inscrire</button>
      </form> -->
    </div>

  </Layout>
</template>


<script>
  export default {
    metaInfo: {
      title: "Formation Simplification de l'information aux usagers",
      meta: [{
        name: "description",
        content: "Pourquoi et comment employer un langage simple et clair pour nos services publics, en explorant les subtilités du fonctionnement de notre cerveau."
      },
      {
        property: "og:title",
        content: "Formation Simplification de l'information aux usagers - DesignGouv"
      },
      {
        property: "og:description",
        content: "Pourquoi et comment employer un langage simple et clair pour nos services publics, en explorant les subtilités du fonctionnement de notre cerveau."
      },
      {
        property: "og:image",
        content: "https://design.numerique.gouv.fr/assets/meta-images/designgouv.png"
      },
      {
        name: "twitter:card",
        content: "summary_large_image"
      },
      {
        name: "twitter:site",
        content: "@Design_Gouv"
      },
      {
        name: "twitter:title",
        content: "Formation Simplification de l'information aux usagers - DesignGouv"
      },
      {
        name: "twitter:description",
        content: "Pourquoi et comment employer un langage simple et clair pour nos services publics, en explorant les subtilités du fonctionnement de notre cerveau."
      },
      {
        name: "twitter:image",
        content: "https://design.numerique.gouv.fr/assets/meta-images/designgouv.png"
      }],
    },
    data () {
      return {
        form: {
          email: '',
          organisme: '',
          session: [
          "recWbUK6bIoRhCHcb"
        ],
        }
      }
    },
    methods: {
      addParticipant() {
        document.getElementById('submit').disabled = true;
        var Airtable = require('airtable');
        var base = new Airtable({apiKey: process.env.GRIDSOME_AIRTABLE_API_KEY}).base(process.env.GRIDSOME_AIRTABLE_COURSE_BASE);
        base('Inscriptions').create([
        {
          "fields": {
            "E-mail": this.form.email,
            "Organisme": this.form.organisme,
            "Session": this.form.session,
          }
        },
      ], function(err, records) {
        if (err) {
          window.location.href = "/formulaire/erreur/";
          console.error(err);
          return;
        } else {
          window.location.href = "/formulaire/succes/";
        }
      });
    }
  },
}
</script>


<style scoped lang="scss">

  @import "src/assets/scss/_vars.scss";

  .person {
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    margin-bottom: 2rem;

    &__photo {
      height: 7rem;
      width: 7rem;
      border-radius: 50%;
      margin-right: 2rem;
      flex-basis: auto;
    }

    &__description {
      flex-basis: 20rem;
      margin: 0.5rem 0;
    }
  }

</style>
