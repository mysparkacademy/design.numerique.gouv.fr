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
              <span aria-current="page">Formation à l’accessibilité</span>
            </li>
          </ol>
        </nav>
        <h1 class="dg-cover__title">Formation à l’accessibilité</h1>
        <p class="fr-text--lead">Pourquoi et comment bien prendre en compte les personnes en situation de handicap dans la conception de services publics numériques.</p>
      </div>
    </div>

    <div class="dg-content dg-content--xs fr-px-2w fr-mt-6w">
      <h2>Revivez la formation en vidéo</h2>
      <p>La formation a eu lieu en direct le jeudi 18 novembre. Vous pouvez la revivre <a href="https://www.youtube.com/watch?v=_5zIrh-LDto" target="_blank" title="sur notre chaîne YouTube - Nouvelle fenêtre">sur notre chaîne YouTube</a>.</p>

      <h3>Objectifs</h3>
      <ul>
        <li>S’approprier les concepts de l’accessibilité d’un point de vue historique et juridique</li>
        <li>Connaître les obligations, identifier les rôles et responsabilités</li>
        <li>S’organiser et disposer d’une boîte à outils</li>
      </ul>

      <h3>Public concerné</h3>
      <p>Agents de la fonction publique ou prestataires impliqués dans la conception des démarches administratives numériques.</p>

      <h3>Programme</h3>
      <ul>
        <li>Immersion</li>
        <li>Un peu d’histoire</li>
        <li>Démonstration</li>
        <li>Définition et dispositif légal</li>
        <li>Prévalence du handicap</li>
        <li>Le référentiel général d’amélioration de l’accessibilité (RGAA)</li>
        <li>Méthodes et outils</li>
      </ul>
      <p>C’est important, c’est gratuit, c’est ludique, c’est opérationnel et c’est toujours disponible <a href="https://www.youtube.com/watch?v=_5zIrh-LDto" target="_blank" title="sur notre chaîne YouTube - Nouvelle fenêtre">sur notre chaine Youtube</a> !</p>
      <p>N'oubliez pas, nous proposons d’autres formations : <g-link to="/formations/design/">design</g-link>, <g-link to="/formations/recherche-utilisateur/">recherche utilisateur</g-link>, <g-link to="/formations/ecoconception/">écoconception</g-link> et <g-link to="/formations/simplification-information/">simplification de l’information</g-link>.</p>
    </div>

  </Layout>
</template>


<script>
  export default {
    metaInfo: {
      title: "Formation à l'accessibilité",
      meta: [{
        name: "description",
        content: "Pourquoi et comment bien prendre en compte les personnes en situations de handicap dans la conception de services publics numériques"
      },
      {
        property: "og:title",
        content: "Formation à l'accessibilité - DesignGouv"
      },
      {
        property: "og:description",
        content: "Pourquoi et comment bien prendre en compte les personnes en situations de handicap dans la conception de services publics numériques"
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
        content: "Formation à l'accessibilité - DesignGouv"
      },
      {
        name: "twitter:description",
        content: "Pourquoi et comment bien prendre en compte les personnes en situations de handicap dans la conception de services publics numériques"
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
          formation: 'Accessibilité',
          session: '2021-11-18'
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
            "Formation": this.form.formation,
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
