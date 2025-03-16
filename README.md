node -e "try { require('fs'); console.log('Modules OK') } catch(e) { console.log('Thiếu module:', e.message.match(/'(.+?)'/)[1]) }"
