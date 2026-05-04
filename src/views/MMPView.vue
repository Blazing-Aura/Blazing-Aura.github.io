<script setup lang="ts">
import SplitLayout, { type layoutData } from '@/components/SplitLayout.vue'

const AboutProject: layoutData = {
  primaryImage: 'images/MMP_Context.svg',
  imageAlt:
    'Image of the Mindfulness Motion Pets Home page being shown on a phone, with a person holding it in their hand.',
  leftSide: true,
}

const ProjectProcess: layoutData = {
  primaryImage: 'images/MMP_Process.png',
  imageAlt:
    'Screenshot of multiple pages of the design documentation for the Mindfulness Motion Pet project, including photo`s and drawings done.',
  leftSide: false,
}

const LearnMore: layoutData = {
  primaryImage: 'images/MMP_Final.png',
  imageAlt:
    'Image of all the Mindfulness Motion Pets final UI`s shown in a structured slanted layout.',
  leftSide: true,
}
</script>

<template>
  <div class="hero-section">
    <h1>Mindfulness Motion Pet</h1>
  </div>
  <SplitLayout :required-data="AboutProject">
    <h2>What's the problem?</h2>
    <p>
      Through research, there is still a gap in supporting those impacted by mental illnesses. The
      problem identified was: how might we design an engaging and valuable app that promotes
      positive mental well-being to support those impacted by depression, anxiety and bipolar
      disorder?
    </p>
    <h3>The outcome</h3>
    <ul>
      <li>
        Developed a prototype phone app to support those with mental illnesses and promote positive
        mental well-being
      </li>
      <li>
        Facilitate the possibility of adopting a real pet to continue their journey for a positive
        lifestyle.
      </li>
    </ul>
    <h3>What skills did i learn?</h3>
    <ul>
      <li>
        Following an iterative process that allows for discussion and helps develop or adjust the
        idea to better succeed its intended purpose. (working more as a collaborative environment
        than individually)
      </li>
      <li>
        Designing in the health sector requires great attention to detail to make sure the idea has
        no unintended consequences for its users.
      </li>
    </ul>
  </SplitLayout>
  <SplitLayout :required-data="ProjectProcess">
    <h2>Design Process</h2>
    <p>
      Through the development of the project, i firstly broke down the problem and did some
      introductory research to understand where to begin for the contextual research. With
      contextual research, there was three topics which were researched, which included apps
      focusing on mental well-being, physiotherapy and pet therapy. Next began the ideation, which
      based on the research conducted, combining each idea would result in the best of all worlds.
      This would result in the initial concept Mindfulness Valuable Pet. Before the final prototype
      could begin to be developed, both a user empathy map and user persona's were needed to
      understand the theoretical needs and wants of the target audience, therefore making sure the
      prototype would be addressing the problem.
    </p>
    <p>
      With the idea features combined, Mindfulness Motion Pet was created to incorporate an AR
      virtual pet that could provide positive activities to the participant and provide other
      beneficial information when needed. Before creating the prototype on Figma, wireframes were
      needed to provide an idea as to how the app would be structured out, and if there would be any
      final adjustments.
    </p>
    <h3>
      For further details, or if you wanted to look at the entire design documentation, feel free to
      ask!
    </h3>
  </SplitLayout>
  <SplitLayout :required-data="LearnMore">
    <h2>Final solution</h2>
    <p>
      In the limited amount of time provided to create the prototype, it was decided that it would
      be done on Figma to facilitate a level of interactivity that can be used for further user
      testing to verify that the idea would work as intended for its target audience.
    </p>
    <p>
      The Figma
      prototype demonstrates a phone app that would promote an active user through a virtual pet
      that would encourage the user to complete tasks and congratulate the user when they complete
      specific tasks. There is also an Augmented Reality feature providing the user with the chance
      to further engage with their virtual pet, while leading to the possibility of adopting a furry
      friend, depending on the animal the user chose to be their buddy.
    </p>
  </SplitLayout>
</template>

<style scoped>
/* styling for the hero image section */
.hero-section {
  background-image: url(../../public/images/MMP_hero.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  width: 100%;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: left;
  text-align: left;

  & h1 {
    width: fit-content;
    max-width: 55%;
    font-size: 8rem;
    color: var(--white);
    background-color: rgba(116, 116, 116, 0.75);
    padding: 0 0 var(--padding-large) var(--padding-large);
    transition: color 2s;
  }

  & h1:hover {
    color: var(--complement-colour);
  }
}

/* keyframes for making the header text change colour slightly */
@keyframes color-header {
}
</style>
