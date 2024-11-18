# React - dom

### Code to implements react-dom to your html
    
    <script  src="https://unpkg.com/react@18/umd/react.development.js"></script> 
    <script  src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>

Instead of directly manipulating the DOM with plain JavaScript, remove the DOM methods that you had added previously, and add the [`ReactDOM.createRoot()`](https://react.dev/reference/react-dom/client/createRoot) method to target a specific DOM element and create a root to display your React Components in. Then, add the [`root.render()`](https://react.dev/reference/react-dom/client/hydrateRoot#root-render) method to render your React code to the DOM. 

---
### Example how to  implements react-dom

    <script> 
	    const app = document.getElementById('app');
	    const  root = ReactDOM.createRoot(app);
	    root.render(<h1>Hello, World! This is NextJS_StudyRepo.</h1>)
    </script>
   > But this will result you an error because JS can't handle **HTML tag** 