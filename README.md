First Laravel App - beginners

1) create new laravel project: laravel_app

2) make all database connection setup, do artisan migrate

3) blade templating and layout
   a) Setting vite and tailwindcss
      - npm install
      - npm run dev

          VITE v6.0.11  ready in 892 ms

          ➜  Local:   http://localhost:5173/
          ➜  Network: use --host to expose
          ➜  press h + enter to show help

          LARAVEL v11.41.0  plugin v1.2.0

          ➜  APP_URL: http://localhost
      
      - vite will watch for any changes in html, css or javascript
        and refresh the app directly in the browser

          ➜  APP_URL: http://localhost
        10:52:40 AM [vite] full reload resources\views\welcome.blade.php
        10:52:40 AM [vite] (client) page reload resources/views/welcome.blade.php
        10:52:40 AM [vite] (client) page reload storage/framework/views/752176d51c1315fcec1d5fba437c33b9.php 

    b) configure tailwindcss
       - stop npm run dev 
       - npm install tailwindcss @tailwindcss/vite
       - edit tailwind.config.js
         
         /* import */
         import { defineConfig } from 'vite'
         import tailwindcss from 'tailwindcss'
         import defaultTheme from 'tailwindcss/defaultTheme'; 

         /* plugins */
         plugins: [tailwindcss()],

       - run: npm run dev