## Exercise 1 - Create Your Own React App

**Goal:** We set up our own React app, which we will use as a basis for a memory game that we will implement throughout 
this workshop.

### Steps
1. Go to the CoderPad link we provide for your group. There you can join a session allowing everyone in the group 
   to see and edit the CoderPad concurrently.

2. Set up your CodePad for React
   1. Select "React" from "Languages"
   2. update the package.json to use the latest React and TypeScript versions, it should look like this:
     ```json
     {
        "name": "react-for-e-fellows",
        "private": true,
        "version": "0.0.0",
        "type": "module",
        "dependencies": {
           "react": "^18.2.0",
           "react-dom": "^18.2.0"
        },
        "devDependencies": {
           "@types/node": "^20.0.0",
           "@types/react": "^18.2.0",
           "@types/react-dom": "^18.2.0",
           "@vitejs/plugin-react": "^4.2.0",
           "typescript": "^5.3.0",
           "vite": "^5.0.0"
        }
     }
     ```
   
3. Install the dependencies: Run `npm install` (or short `npm i`) in the CoderPad shell.

4. Adjust `main.tsx` for the latest React version. It should look like this:
   ```tsx
   import { createRoot } from 'react-dom/client'
   import './index.css'
   import App from './App'
   
   const rootElement = document.getElementById("root") as HTMLElement;
   createRoot(rootElement).render(<App />);
   ```

5. Have a look at the generated files:
    * root folder 
    * **src** folder 

6. Try to change something and see the result!

7. Write your own "Hello World" component

---

#### Tip: If you want to try out more at home
On `https://codesandbox.io` you can create small react apps in the browser without having to set up anything on your 
computer, which is ideal for playing around with React and trying out some things. It is similar to Coderpad, but also 
offers free access (live-collaboration is however not free). 
When creating the sandbox, select the "React TypeScript" template.