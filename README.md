# React + Vite

# Clean code and create program structure. Makes it easier to structure and call components and other files into app or main file.

# main dir => public(place logo) 
# main dir => src => assets(icons, images, logo and call logo from assets dir)(also add index.js in both assets and icons dirs) 
#src => components(Nav, Footer, index.js, Other files that will be used by the program, e.g. ShoeCard, Button, etc) In the components/index.js Add imports of all components inside the index.js and export all components also in the components/index.js
#src => constants(index.js(add footer, nav links, social media links, and import, etc))
#src => sections(OPTIONAL DIR. THE FILES INSIDE sections dir can also be all put inside components dir. The sections dir will contain files such as Hero, Footer, Services, CustomerReviews, index.js, etc. THESE CAN ALL BE PUT INSIDE THE COMPONENTS DIR. THEREFORE THE SECTIONS DIR IS AN OPTIONAL DIR AS ALL FILES INSIDE IT CAN ALL BE INCLUDED INSIDE THE COMPONENTS DIR)
#src => App.jsx, main.jsx, index.css
#main dir =>.eslintrc(default file, .gitignore(include password files, sensitive info to be excluded when launching app online), package.json, and other default files

#.npm create vite@latest ./ -- --template react
#.install and config tailwind. npm install -D tailwindcss postcss autoprefixer
#.npx tailwindcss init -p
#.copy and paste from tailwindcss.com the tailwind utilities and tailwind base file paste into index.css.You can also replace the whole index.css with tailwind utilities
#.from tailwindcss.com/docs/guides/vite copy from app.jsx the code and replace it with the one in app.jsx of the application
#.delete app.css
#.add your own assets folder
#.create files in components dir 
#.in the App.jsx import components and add them inside the const App = () => () code block as such:
const App = () => (
  <main className="relative">
    <Nav /> 
    <section className="xl:padding-1 wide:padding-r padding-b">
      <Hero />
    </section>
    <section className="padding">
      <PopularProducts />
    </section>
    <section className="padding">
      <SuperQuality />
    </section>
  <main>
  
#in the end run the cmd npm run build to build the program for production and deploy online

