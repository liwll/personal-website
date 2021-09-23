<template>
    <div class="projects">
        <h1>Projects</h1>
        <div class="project" v-for="project in projects" :key="project.id">
            <a class="name" :href=project.link target="_blank" rel="noopener noreferrer">
                {{ project.name }} <i class="bi bi-link-45deg"></i>
            </a>
            <div class="description">
                {{ project.description }}
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Projects',
    data() {
        return {
            projects: [
                {
                    id: 0,
                    name: 'Covid Simulation',
                    description: 'A web app featuring several visualizations and an interactive simulation which demonstrates how to "flatten the curve" through vaccinations and social distancing.',
                    link: 'https://github.com/liwll/covid-sim-vizathon-2021',
                },
                {
                    id: 1,
                    name: 'Todo List',
                    description: 'Organize your tasks with todo lists in this app.',
                    link: 'https://github.com/liwll/todo-list',
                },
                {
                    id: 2,
                    name: 'Reaction Timer Game',
                    description: 'A simple web app which measures your visual reaction time.',
                    link: 'https://github.com/liwll/reaction-timer-game',
                },
                {
                    id: 3,
                    name: 'Restaraunt Page',
                    description: 'A restaurant page template with a home, menu, and about page.',
                    link: 'https://github.com/liwll/restaurant-page',
                },
                {
                    id: 4,
                    name: 'Tic-Tac-Toe',
                    description: 'A simple Tic-Tac-Toe game for two players.',
                    link: 'https://github.com/liwll/tic-tac-toe',
                }
            ]
        }
    },
}
</script>

<style scoped>
h1 {
  border-bottom: 1px solid #228b22;
  padding-bottom: 0.25em;
}
.projects {
    display: block;
    margin: 5em auto;
    width: 50%;
}
.project {
    margin: 1em 0;
    border-left: 1px solid #228b22;
    padding: 15px;
}
.name {
    font-size: 1.7em;
    cursor: pointer;
    transition: 100ms ease-in-out;
}
.name:hover {
    font-size: 1.75em;
}
a:visited, a:link {
  color: inherit;
  text-decoration: none;
}
.description {
    margin-top: 15px;
    word-wrap: break-word;
}
</style>