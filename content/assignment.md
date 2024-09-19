---
title: Rick & Morty and Pokémon Overview Application
description: Instructions for the Rick & Morty and Pokémon Overview Application assignment
---

# Assignment: Rick & Morty and Pokémon Overview Application

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

- **Unique Detail Pages**: Each character or Pokémon should have a dedicated detail page that is navigable from the overview.
- **Consistent Layout**: The layout of Rick & Morty character detail pages should be structurally identical to Pokémon detail pages, focusing only on presenting the appropriate content.

### Bonus Points

- **View Modes**: Implement a grid or list view toggle option for the overviews.
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

4. **Two-Way Data Binding**
   - If you need to share states between different components, use `v-model` or similar mechanisms for reactive state binding between parent and child components. Make sure to handle the data flow correctly, and avoid anti-patterns.
5. **Project structure**
   - Ensure your project structure is clean and organized. Use folders and files to separate concerns and keep your codebase maintainable.

---

## Technical Requirements

- **State Management**: Use Pinia for state management. It is already installed. Refer to [Pinia documentation](https://pinia.vuejs.org/) for usage.

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

- The repository is called **"boilerplate"** for a reason. We'd like to see how you would **add your design sauce** to the mix. Feel free to incorporate your own unique styling, animations, or other creative elements that align with best practices.
- Ensure consistency and good UX practices, but bring your own flavor into the design.
- Always look for existing modules before installing packages.
- The above pointers and best practices are **non-negotiable**.
- Commit early, commit often. We'd like to see your progress as you work through the assignment. This also helps us understand your thought process.
- **Have fun!** We're excited to see what you come up with. If you have any questions, feel free to reach out to us.

---
