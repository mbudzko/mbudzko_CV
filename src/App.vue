<script setup>
import SkillChip from "./components/SkillChip.vue";
import WorkCard from "./components/WorkCard.vue";

const skills = ['VueJs', 'Vue2', 'Vue3', 'Javascript', 'NodeJS', 'Tailwind', 'Bootstrap', 'Typescript', 'Vite', 'Nuxt', 'Vuex', 'Pinia', 'Jest', 'Vuetify', 'Quasar', 'C#', '.NET', 'Python', 'KonvaJs', 'Canvas', 'HTML5', 'CSS', 'SCSS', 'SASS'];
const secondary = ['Git', 'npm', '(yarn/pnpm)', 'Github', 'Azure', 'Gitlab', 'CI/CD', 'Webpack', 'Babel', 'Responsive Design', 'SSR', 'ESR', 'PWA', 'TDD', 'Agile', 'Jira/Confluence', 'ClickUp', 'VSCode', 'Webstorm',]

const jobs = [
  {
    title: 'Staar Surgical',
    position: 'Senior Software Engineer',
    description: 'Fullstack development across multiple projects, mainly focused on maintaining and improving the main product made up of several web applications. Tasks include working on frontend architecture, adding new features, and coordinating with other teams. Also responsible for creating and updating internal tools to support daily operations. Work involves regular collaboration with the customer service team to handle user issues, improve workflows, and keep the product stable.',
    startDate: 'June 2024',
    endDate: 'Current',
    linkedinLink: 'https://www.linkedin.com/company/staar-surgical',
    type: 'Full Time',
  },
  {
    title: 'Lambda Factor',
    position: 'Senior Software Engineer',
    description: 'Consulting, different types of projects.',
    startDate: 'April 2024',
    endDate: 'Current',
    linkedinLink: 'https://www.linkedin.com/company/lambdafactor',
    type: 'Part Time',
  },
  {
    title: 'SenseHawk, Inc',
    position: 'Senior Software Engineer',
    description: 'Module owner. Development of the owned module, integration with other modules, prototyping, planning, components development, development and integration of new features, working with a product and design teams, support of the product.',
    startDate: 'October 2022',
    endDate: 'Feb 2024',
    linkedinLink: 'https://www.linkedin.com/company/sensehawk',
    type: 'Full Time',
  },
  {
    title: 'IntexSoft',
    position: 'Software Engineer, Senior Software Engineer',
    description: 'Variety of different projects, mostly commercial web applications. Several big projects including NFT market platform. Working with different teams, leading a team at some point.',
    startDate: 'September 2020',
    endDate: 'October 2022',
    linkedinLink: 'https://www.linkedin.com/company/intexsoft',
    type: 'Full Time',
  },
  {
    title: 'INSPR',
    position: 'Software Engineer',
    description: 'Fullstack development of the framework based on React library',
    startDate: 'October 2019',
    endDate: 'September 2020',
    linkedinLink: 'https://www.linkedin.com/company/insprlabs',
    type: 'Full Time',
  }
]
</script>

<template>
  <div class="page">
    <div class="main-info ta-start">
      <div class="title">
        <h1 style="margin: 0;">
          Maksim Budzko
        </h1>
        <h2>Senior Software Engineer</h2>
      </div>
      <section>
        <h3>
          SUMMARY
        </h3>
        <p>
          Frontend Engineer with over 6 years of experience working with Vue.js, using both the Composition and Options APIs. I enjoy solving problems and finding practical, creative solutions to complex tasks. I’m known for being reliable, easy to work with, and comfortable collaborating in different team setups. I’ve worked on a wide range of projects with various architectures, and I adapt quickly to new environments while keeping quality and efficiency high.
        </p>
      </section>

      <section>
        <h3>
          CAREER ACCOMPLISHMENTS
        </h3>
        <ul>
          <li>
            <p>
              Successfully led several major migrations from Vue 2 to Vue 3, managing the transition smoothly and ensuring the projects continued to run reliably throughout the process.
            </p>
          </li>
          <li>
            <p>
              Guided and mentored a team of frontend developers, helping them grow while fostering a supportive and productive environment.
            </p>
          </li>
          <li>
            <p>
              Took full ownership of a critical module, demonstrating independence, accountability, and a deep understanding of the project’s architecture and dependencies.
            </p>
          </li>
          <li>
            <p>
              Designed and implemented a key backup system to keep services operational and protect data during offline periods throughout a major migration.
            </p>
          </li>
        </ul>
      </section>

      <section>
        <h3>
          SKILLS
        </h3>
        <div style="padding-left: 1rem;">
          <h5 style="margin-bottom: 0;">
            Primary
          </h5>
          <SkillChip
            v-for="skill in skills"
            :key="skill"
            :label="skill"
          />
        </div>

        <div style="padding-left: 1rem;">
          <h5 style="margin-bottom: 0;">
            Methodologies and other
          </h5>
          <SkillChip
            v-for="skill in secondary"
            :key="skill"
            :label="skill"
          />
        </div>
      </section>

      <br>
      <section>
        <h3>
          Experience
        </h3>
        <div>
          <WorkCard
            v-for="job in jobs"
            :key="job.title"
            :title="job.title"
            :position="job.position"
            :description="job.description"
            :start-date="job.startDate"
            :end-date="job.endDate"
            :linkedin-link="job.linkedinLink"
            :type="job.type"
          />
        </div>
      </section>

      <section>
        <h3> Education </h3>

        <div class="education">
          <div class="education__period">
            2017 - 2021
          </div>
          <div>
            <h5>
              Bachelor of Computer Science
            </h5>
            Yanka Kupala State University of Grodno: Mathematics and Informatics faculty, Computer Security.
          </div>
        </div>
      </section>
    </div>
    <div class="secondary-info ta-start">
      <div class="secondary-info__content">
        <h4>
          Contacts
        </h4>
        <div class="subtitle">
          <div>
            Address: Wroclaw, Poland
          </div>
          <div>
            Phone:
            <a href="tel:+48698737515">
              +48698737515
            </a>
          </div>
          <div>
            Email:
            <a href="mailto:budzkomaksim@gmail.com">
              budzkomaksim@gmail.com
            </a>
          </div>
        </div>

        <h4>
          Links
        </h4>
        <div>
          <div>
            Github: <a
              href="https://github.com/mbudzko/"
              target="_blank"
            > https://github.com/mbudzko </a>
          </div>
          <div>
            LinkedIn: <a
              href="https://www.linkedin.com/in/maksim-budzko-388577219/"
              target="_blank"
            > maksim-budzko-388577219 </a>
          </div>
          <div>
            CV Repository: <a
              href="https://github.com/mbudzko/mbudzko_CV"
              target="_blank"
            > Click! </a>
          </div>
        </div>
      </div>

      <div class="remark">
        <div>
          This CV is a small VueJs app
        </div>
        <div>
          Check out web version <a
            href="https://mbudzko.github.io/mbudzko_CV/"
            target="_blank"
          >here</a>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
h3 {
  text-transform: uppercase;
}

a {
  font-weight: 500;
}

.ta-start {
  text-align: start;
}
.page {
  width: 100%;
  display: grid;
  grid-template-columns: 65% auto;
}
.main-info {
  padding-right: 1rem;
}

.secondary-info {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  position: fixed;
  right: 0;
  bottom: 0;
  top: 0;
  border-left: 1px solid #464646;
  padding: 2rem;
  margin: 1rem;
  height: auto;
}

.education {
  display: flex;
  justify-content: space-between;
  align-items: start;

  &__period {
    margin-right: 1rem;
    white-space: nowrap;
  }

  h5 {
    margin-top: 0;
    margin-bottom: 0.5rem;
  }
}

.remark {
  display: none;
  flex-direction: column;
}

@media screen and (max-width: 900px) {
  .page {
    display: flex;
    flex-direction: column;
  }

  .secondary-info {
    border-left: none;
    border-top: 1px solid;
    margin: 1rem 0;
    padding: 1rem 0;
    position: relative;
    bottom: 0;
    transform: scale(0.7);
  }
}

@media print {
  .secondary-info {
    right: 0;
    bottom: 0;
    top: 0;
    margin: 0;
    margin-left: 5rem;
    padding: 0;
    height: auto;
    &__content {
      transform: scale(0.7);
    }
  }

  .remark {
    display: flex;
    align-self: end;
    transform: scale(0.8);
    flex-direction: column;
  }
}
</style>
