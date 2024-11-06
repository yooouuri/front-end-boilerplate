---
title: Rick & Morty and Pokémon Overview Application
description: Instructions for the Rick & Morty and Pokémon Overview Application assignment
---

# Assignment: Rick & Morty and Pokémon Overview Application

Please read these instructions carefully.

## Objective

Create a Nuxt application to showcase two distinct content overviews:

1. **Rick and Morty characters**
2. **Pokémon**

Each overview must be accessible via a separate page. Selecting an item from an overview should navigate users to a detailed page for that item. The user experience (UX) across overviews and detail pages should be consistent, with only the data changing based on the selected item (Rick & Morty character or Pokémon). Both APIs are integrated in the project, but you may add a third if desired. Refer to the API documentation:

- [Rick and Morty API](https://rickandmortyapi.com/documentation).
- [Pokémon API](https://pokeapi.co/docs/v2).

## Wireframes

You are free to design the application as you see fit, but you can use the following wireframes as a reference:

::content-wireframes
::

---

## Deliverable

Fork this repository and submit your solution as a new repository. Once complete, share the link for review. We’ll provide feedback on your code.

## Requirements

### 1. Overviews

- **Separate Pages**: Each overview (Rick & Morty and Pokémon) should be on its own page.
- **Consistent UI/UX**: The overview and detail pages should maintain a unified design, with the only difference being the displayed data.
- **Navigation**: Clicking an item in the overview should navigate to a detail page with specific information about the selected character or Pokémon.

### 2. Detail Pages

- **Dedicated Detail Pages**: Each character or Pokémon should have its own detail page, navigable from the overview.
- **Component Structure**: Design components with scalability in mind to facilitate adding more overviews in the future without significant rework.
- **View Modes**: Implement grid and list view options for the overviews.
- **Consistent Layout**: The layout for Rick & Morty and Pokémon detail pages should be identical in structure, displaying only the relevant content.

### Bonus Points

- **Unit Testing**: Add one or more unit tests to ensure component functionality and reusability.

---

## Key Development Concepts to Demonstrate

1. **Reusability**

   - Code should be scalable and reusable, with no hard-coding or tight coupling for specific scenarios.

2. **Composition Over Inheritance**

   - Avoid using `if/else` statements for conditional CSS classes; instead, make components as modular and single-purpose as possible. However, it's perfectly acceptable to use `if/else` logic to render different components based on the application state.

3. **Single Responsibility Components**

   - Keep components focused on a single function, avoiding excessive logic or UI in one place when it can be split into smaller modules.

4. **Two-Way Data Binding** (when applicable)

   - If state sharing between components is needed, use `v-model` or similar for reactive state management between parent and child components, ensuring proper data flow and avoiding anti-patterns.

5. **Project Structure**

   - Organize the project structure clearly, using folders and files to separate concerns and maintain a clean codebase.

---

## Technical Requirements

- **State Management**: Use a global state if needed. Pinia is already installed; refer to the [Pinia documentation](https://pinia.vuejs.org/) for guidance. You can also consider using `provide` and `inject` with VueUse if appropriate. Managing the view mode (grid or list) for each overview could be a good use of state.

- **API Integration**: Handle data fetching through the API Party composables. Refer to the [API Party documentation](https://example.com/api-party) for guidance. The current landing page includes an example.

- **UI Components**: Use components from [Nuxt UI](https://ui.nuxt.com/) to maintain design consistency. Tailwind CSS is pre-configured and can be customized as needed.

## Additional Resources

- **VueUse Functions**: VueUse composables are auto-imported. Use them as needed—check the [VueUse documentation](https://vueuse.org/) for more information.

- **Nuxt & Vue**: Ensure that your components, pages, and logic align with Nuxt and Vue.js best practices.

---

## TypeScript

If you choose to use TypeScript:

- **Scalable Usage**: Ensure that your TypeScript implementation is scalable, reusable, and follows best practices.

---

## Final Guidelines

- **Enjoy the Project!** We’re excited to see your approach to the challenge. Reach out with any questions.
- **Commit Regularly**: Make frequent commits for better version control.
- **Package Manager**: The project specifies `pnpm` in `package.json`. If you prefer another package manager, you can change it, but please delete the `pnpm` lock file and commit the new one.
- **Netlify Deployment**: You can deploy your project on Netlify, which is pre-configured. Follow the [Netlify documentation](https://docs.netlify.com/site-deploys/create-deploys/) for deployment instructions. If you deploy, set the website address in your repository settings.
- **Linter rules**: We'd prefer you sticking to existing linter rules. These are the rules we use in our projects. If you want to change them, please let us know why.

---

## Getting Started

### 1. Clone to Local Machine

```bash
npx degit spend-cloud-tom/front-end-boilerplate proactive-technical-assessment-my-name
cd proactive-technical-assessment-my-name
pnpm i # If pnpm isn’t installed, run: npm install -g pnpm
```

### 2. Run the Project

```bash
pnpm run dev
```
