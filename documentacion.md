bash
# INICIALIZACIÓN DEL PROYECTO

## Crear y configurar el repositorio inicial

bash
# Crear directorio del proyecto
mkdir proy1
cd proy1

# Configurar Git (si no lo has hecho antes)
git config --global user.name "Tu nombre"
git config --global user.email "tu.email@ejemplo.com"

# Inicializar repositorio
git init

# Crear README.md inicial
echo "# GIS Lima - Gestión de Puntos de Interés" > README.md
echo "" >> README.md
echo "Aplicación web para gestionar puntos de interés en Lima Perú" >> README.md
echo "" >> README.md
echo "## Tecnologías" >>  README.md
echo "- Frontend: HTML, CSS, Javascript, Leaflet, Openlayer" >> README.md
echo "- Backend: Java (Spring Boot), Python, Lenguaje R" >> README.md
echo "- Base de Datos Espaciales: PostgreSQL+Postgis, Oracle Spatial" >> README.md

# Ver estado del repositorio
git status

# Añadir y hacer primer commit
git add README.md
git .  #cuando son muchos archivos
git commit -m "docs: inicializar proyecto GIS Lima POI"

# Verificar historial
git log --oneline

# Modificando el archivo README.md
echo "" >> README.md
echo "SENCICO 2025©" >>  README.md

# Ver estado del repositorio: README.md modificado
git status

# Aplicando las modificaciones
git commit -a -m "docs: Se agregó el año y el logo de SENCICO proyecto GIS Lima POI"

# Subir el repositorio al GitHub
# p1. Crear el repositorio en el GitHub
git branch -M main
git remote add origin https://github.com/anrobe/proy1.git
git push -u origin main
bash