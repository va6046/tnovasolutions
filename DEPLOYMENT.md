# 🚀 Guía de Despliegue - TICNova Solutions

## 📋 Pasos para Subir a GitHub

### 1. Crear Repositorio en GitHub

1. Ve a [GitHub.com](https://github.com) y haz login
2. Haz clic en "New repository"
3. Configura el repositorio:
   - **Nombre:** `tnovasolutions-website`
   - **Descripción:** Sitio web corporativo de TICNova Solutions
   - **Visibilidad:** Public (para GitHub Pages)
   - **NO** inicializar con README (ya tenemos uno)

### 2. Clonar y Configurar Localmente

```bash
# Clonar el repositorio (reemplaza 'tu-usuario' con tu username)
git clone https://github.com/tu-usuario/tnovasolutions-website.git
cd tnovasolutions-website

# Copiar todos los archivos del proyecto aquí
# (index.html, styles.css, script.js, logos, etc.)

# Agregar archivos al staging
git add .

# Hacer commit inicial
git commit -m "Initial commit: TICNova Solutions website"

# Subir al repositorio
git push -u origin main
```

### 3. Configurar GitHub Pages

1. Ve a tu repositorio en GitHub
2. Haz clic en **Settings**
3. Scroll hacia abajo hasta **Pages**
4. En **Source**, selecciona **Deploy from a branch**
5. Selecciona **main** branch y **/ (root)**
6. Haz clic en **Save**

### 4. Configurar Dominio Personalizado

1. En la sección **Pages**, busca **Custom domain**
2. Ingresa: `tnovasolutions.com`
3. Marca **Enforce HTTPS**
4. Haz clic en **Save**

### 5. Configurar DNS

En tu proveedor de dominio, configura estos registros DNS:

```
Tipo: A
Nombre: @
Valor: 185.199.108.153

Tipo: A  
Nombre: @
Valor: 185.199.109.153

Tipo: A
Nombre: @
Valor: 185.199.110.153

Tipo: A
Nombre: @
Valor: 185.199.111.153

Tipo: CNAME
Nombre: www
Valor: tu-usuario.github.io
```

### 6. Verificar Despliegue

- **GitHub Pages URL:** `https://tu-usuario.github.io/tnovasolutions-website`
- **Dominio personalizado:** `https://tnovasolutions.com`

## 🔧 Comandos Git Útiles

```bash
# Ver estado de archivos
git status

# Agregar archivos específicos
git add index.html styles.css script.js

# Agregar todos los archivos
git add .

# Hacer commit con mensaje
git commit -m "Descripción del cambio"

# Subir cambios
git push origin main

# Ver historial de commits
git log --oneline

# Crear nueva rama
git checkout -b nueva-funcionalidad

# Cambiar a rama main
git checkout main

# Fusionar rama
git merge nueva-funcionalidad
```

## 📁 Archivos Incluidos

```
✅ index.html              # Página principal
✅ styles.css              # Estilos CSS
✅ script.js               # JavaScript
✅ logo.svg                # Logo principal
✅ logo-compact.svg        # Logo compacto
✅ favicon.svg             # Favicon
✅ robots.txt              # SEO
✅ sitemap.xml             # Mapa del sitio
✅ CNAME                   # Dominio personalizado
✅ .gitignore              # Archivos a ignorar
✅ README.md               # Documentación
✅ README-LOGOS.md         # Documentación de logos
✅ domain-config.md        # Configuración del dominio
✅ DEPLOYMENT.md           # Esta guía
✅ .github/workflows/      # CI/CD
```

## 🎯 Próximos Pasos

1. **Configurar Analytics** (Google Analytics)
2. **Configurar Search Console** (Google Search Console)
3. **Configurar Email** empresarial
4. **Configurar SSL** (automático con GitHub Pages)
5. **Monitorear rendimiento**

## 🆘 Solución de Problemas

### Error 404 en GitHub Pages
- Verificar que el archivo `index.html` esté en la raíz
- Verificar que la rama esté configurada correctamente

### Dominio no funciona
- Verificar registros DNS (puede tomar hasta 24 horas)
- Verificar que el archivo `CNAME` esté presente

### HTTPS no funciona
- Esperar a que GitHub configure el certificado SSL
- Verificar que "Enforce HTTPS" esté habilitado

## 📞 Soporte

Para problemas técnicos:
- **GitHub Issues:** Crear un issue en el repositorio
- **Email:** info@tnovasolutions.com

---

**¡Tu sitio web estará en línea en unos minutos! 🎉**

