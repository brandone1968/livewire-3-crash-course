<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## Livewire 3 crash course

Corso base di Laravel Livewire 3 da usare come riferimento

- [Corso originale su Youtube](https://www.youtube.com/watch?v=c8pPND7kclg&list=PL4cUxeGkcC9htKcjQPGQQL3fQHbIxXowN&index=1).

## Installazione

### Scaricare app

Scaricare e scompattare lo zip da github.  
composer install  
sail up -d  
NB. Se Sail non c'è devi aggiungere sail con:  
- **composer require laravel/sail --dev**  
- **php artisan sail:install**  

### Configura alias Sail  
Configura un alias della shell per semplificare l'esecuzione dei comandi Sail.  
alias sail='vendor/bin/sail'  
oppure  
alias sail='sh $([ -f sail ] && echo sail || echo vendor/bin/sail)'   

#### Per rendere permanente l'alias in Ubuntu  
apri il file di configurazine della shell bash  
*nano ~/.bashrc*     
aggiungi al fondo questa riga  
*alias sail='bash vendor/bin/sail'*    
salva ed esci  
quindi o chiudi il terminale e lo riapri o lanci *source ~/.bashrc*  

### Configura .env
Controlla che il file .env sia presente, altrimenti duplica e rinomina quello di esempio
### Crea la chiave
sail php artisan key:generate  

### Esegui Sail e npm
sail npm install
sail npm run dev
sail php artisan migrate --seed

NB. Se nelle impostazioni la password e una stringa vuota ti avvisa. Ti chiederà anche se vuoi creare il db sqlite  

## GIT - portare il progetto su GitHub
Creare su GitHub un progetto  
accedere alla directory del progetto e lanciare il comando  
git init
git add .
git commit -m "Primo commit"
git remote add origin https://github.com/brandone1968/livewire-3-crash-course.git
git push -u origin main 

git push -f origin main	PER FORZARE NEL CASO IL REPOSITORI DI DESTINAZIONE CONTENGA QUALCOSA, ANCHE SOLO UN README.md  


## Languages and Tools:

<p align="left"> <a href="https://git-scm.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://laravel.com/" target="_blank" rel="noreferrer"> <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/laravel/laravel-original.svg" alt="laravel" width="40" height="40" /> </a> <a href="https://www.linux.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/> </a> <a href="https://www.php.net" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/php/php-original.svg" alt="php" width="40" height="40"/> </a> <a href="https://tailwindcss.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/tailwindcss/tailwindcss-icon.svg" alt="tailwind" width="40" height="40"/> </a> </p>
