# Assignment: Rick & Morty and Pokémon Overview Application

Please read this assignment very well!

## Objective

Create a Nuxt application that showcases two distinct overviews:

1. **Rick and Morty characters**
2. **Pokémon**

Each overview must be accessible via its respective page. Upon selecting an item from an overview, users will be redirected to a detail page. The look, feel, and navigation across the overviews and detail pages must be consistent. The only difference should be the data displayed depending on the content (Rick & Morty characters or Pokémon). Both APIs are already integrated into the project. If you want to add a third one, you can do so. You can look up the specs of both APIs.

- [rickandmortyapi.com](https://rickandmortyapi.com/documentation)
- [pokeapi.co](https://pokeapi.co/docs/v2).

---

## Deliverable

Please fork this repository and submit your solution as your own repository. Once you're done, share the link with us. We will review your code and provide feedback.

## Requirements

### 1. Overviews

- **Separate Pages**: Both Rick & Morty and Pokémon overviews must be displayed on individual pages.
- **Consistency**: Overviews and detail pages should have consistent UI/UX, differing only by the data presented.
- **Navigation**: Clicking an item in the overview should navigate the user to a detail page with specific information about the selected character or Pokémon.

### 2. Detail Pages

- **Unique Detail Pages**: Each character or Pokémon should have a dedicated detail page that is navigable from the overview. Because the overviews should look the same, and only the content differs, you should think about how to structure your components to achieve this. Ask yourself: "What is the same, and what is different?", and also "How can I make this scalable?". In the future, we might want to add more overviews, so we should be able to do so without much hassle.
- **View Modes**: Implement a grid or list view toggle option for the overviews.
- **Consistent Layout**: The layout of Rick & Morty character detail pages should be structurally identical to Pokémon detail pages, focusing only on presenting the appropriate content.

### Bonus Points

- **Unit Testing**: Implement one or more unit tests to ensure correct functionality and reusability of your components.

---

## Key Development Concepts to Demonstrate

1. **Reusability**

   - Your code should be scalable and reusable across multiple scenarios.
   - Avoid hard-coding or tightly coupling logic to specific scenarios.

2. **Composition Over Inheritance**

   - Avoid using conditionals (e.g., `if/else`) to handle different UI presentations in a single component.
   - Ensure each component has a **single responsibility**, and create separate components for distinct tasks.

3. **Single Responsibility Components**

   - Keep components focused and separated. Avoid putting too much logic or UI in one place when it can be modularized.

4. **Two-Way Data Binding** (only when applicable to your solution)

   - If you need to share states between different components, use `v-model` or similar mechanisms for reactive state binding between parent and child components. Make sure to handle the data flow correctly, and avoid anti-patterns.

5. **Project structure**
   - Ensure your project structure is clean and organized. Use folders and files to separate concerns and keep your codebase maintainable.

---

## Technical Requirements

- **State Management**: If you feel you need to use a global state, which is a possibility, you can do this in many ways. If you want to go for Pinia, know that it is already installed. Refer to [Pinia documentation](https://pinia.vuejs.org/) for usage. Another possibility could be to use the provideInjectionState hook offered by vueUse. One of the areas where having a state would be beneficial is to keep track of which overview has which view mode (grid or list).

- **API Integration**: Data fetching should be handled via the API Party composables. Read [API Party documentation](https://example.com/api-party) for guidelines on how to use it effectively. The current landing page already has a sample implementation.

- **UI Components**: Leverage components from [Nuxt UI](https://ui.nuxt.com/) to ensure a cohesive look and feel. Tailwind CSS is pre-configured for styling, and you can adjust its settings as needed.

## Extra pointers

- **VueUse Functions**: VueUse composables are auto-imported. You can use them as needed by referring to the [VueUse documentation](https://vueuse.org/).

- **Nuxt & Vue**: This project uses [Nuxt](https://nuxt.com/) built on top of [Vue.js](https://vuejs.org/). Ensure all components, pages, and logic are in line with Nuxt and Vue.js best practices.

---

## TypeScript

If using TypeScript:

- **Mindful Usage**: Ensure your TypeScript usage is scalable, reusable, and aligns with modern best practices.

---

## Additional Guidelines

- **Have fun!** We're excited to see what you come up with. If you have any questions, feel free to reach out to us.
- The package manager is defined in package.json as pnpm. If you prefer to use bun, npm or yarn, you can change it, but please make sure to remove the pnpm lock file and commit the new one.
- **Commits**: If possible, please commit more often than once.

---

## Getting started

### 1. Clone to local

```bash
npx degit spend-cloud-tom/front-end-boilerplate proactive-technical-assessment-my-name
cd proactive-technical-assessment-my-name
pnpm i # If you don't have pnpm installed, run: npm install -g pnpm
```

### 2. Run the project

```bash
pnpm dev
```

### 3. Deploy on Netlify

You can choose to deploy your project on Netlify. The project is already set up for deployment on Netlify. You can follow the instructions in the [Netlify documentation](https://docs.netlify.com/site-deploys/create-deploys/) to deploy your project. If you do, you can set the website address in the settings of your repository.
