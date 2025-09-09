# Uzence-assignment


This project contains **two reusable React components** built with **TypeScript**:

1. **InputField** – Flexible input component with labels, helper text, error messages, variants, sizes, loading state, clear button, and password toggle.  
2. **DataTable** – Table component with sorting, selectable rows, loading & empty states.  

The project is documented with **Storybook** and includes **basic tests** using **Vitest** and **Testing Library**.  

---

## Table of Contents

- [Project Setup](#project-setup)  
- [Scripts](#scripts)  
- [Testing](#testing)  
- [Storybook](#storybook)  
- [Folder Structure](#folder-structure)  
- [Deployment](#deployment)  
- [Approach](#approach)  
- [Screenshots / GIFs](#screenshots--gifs)

---

## Project Setup

1. **Clone the repository**

```
git clone <YOUR_REPO_URL>
cd react-components-assignment
```

2.  **Install dependencies**
    
`npm install` 

3.  **Start development server**
    

`npm run dev` 

> Opens the app in development mode using Vite.

## Scripts

| Command | Description |
|--|--|
| `npm run dev` | Starts Vite development server |
| `npm run build` |Builds production-ready app |
| `npm run preview` | Preview production build |
| `npm run storybook`| Start Storybook in development mode |
| `npm run build-storybook`| Build static Storybook site (`storybook-static/`) |
| `npm run test:watch` | Run all Vitest tests |
| `npm run test:ui` |Open Vitest interactive test UI |

## Testing

-   Uses **Vitest** with **@testing-library/react** for component testing.
    
-   Basic tests cover:
    
    -   Rendering of components
        
    -   Props functionality (like `disabled`, `loading`, `invalid`)
        
    -   User interactions (e.g., row selection in `DataTable`, clear button in `InputField`)
        

**Run all tests:**

`npm run test` 

**Run in watch mode:**

`npm run test:watch` 

**Open Vitest UI dashboard:**

`npm run test:ui`

## Storybook

-   Components are documented with **Storybook**.
    
-   Run Storybook locally:
    

`npm run storybook` 

-   Build static Storybook site:
    

`npm run build-storybook` 

-   The static site is output in `storybook-static/` and can be deployed to **Vercel, Netlify, or Chromatic**.
    

**Storybook Preview Link:** [Your Storybook Link Here](#)

----------

## Folder Structure

UZENCE-COMPONENTS/
├─ src/
│  ├─ components/
│  │  ├─ inputfield/
│  │  │  ├─ inputfield.tsx
│  │  │  ├─ inputfield.stories.tsx
│  │  │  ├─ inputfield.test.tsx
│  │  ├─ datatable/
│  │  │  ├─ datatable.tsx
│  │  │  ├─ datatable.stories.tsx
│  │  │  ├─ datatable.test.tsx
│  ├─ App.css
│  ├─ App.tsx
│  ├─ index.css
│  ├─ index.tsx
├─ stories/
├─ node_modules/
├─ public/
├─ .storybook/
├─ storybook-static/
├─ package.json
├─ package-lock.json
├─ tsconfig.json
├─ vite-env.d.ts
├─ vitest.config.ts
├─ README.md


----------

## Deployment

1.  Build Storybook:
    

`npm run build-storybook` 

2.  Deploy `storybook-static/` folder to a hosting service:
    

-   **Vercel:** `vercel deploy storybook-static --prod`
    
-   **Netlify:** Set **Publish directory** to `storybook-static`
    
-   **Chromatic:** Connect Storybook for cloud hosting & visual regression testing
    

3.  Include the **preview link** in your submission.
    

----------

## Approach

-   Components are **fully typed with TypeScript**.
    
-   Styled with **Tailwind CSS** for consistency and modern design.
    
-   **Basic accessibility** implemented using ARIA attributes.
    
-   Testing ensures components behave correctly with different props and user interactions.
    
-   Storybook documents all interactive states, variants, and sizes.
    

----------


