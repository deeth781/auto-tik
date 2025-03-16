node -e "try { require('fs'); console.log('Modules OK') } catch(e) { console.log('Thiếu module:', e.message.match(/'(.+?)'/)[1]) }"
pkg install python3 make gcc nodejs-lts -y
npm install -g node-gyp
cd ~/auto-tik
rm -rf node_modules package-lock.json  
npm cache clean --force  
npm install sqlite3 --build-from-source  
