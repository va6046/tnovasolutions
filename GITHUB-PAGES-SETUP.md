# Configuración de GitHub Pages

## Pasos para Configurar GitHub Pages

### 1. Habilitar GitHub Pages en el Repositorio

1. Ve a tu repositorio en GitHub: `https://github.com/va6046/tnovasolutions`
2. Haz clic en **Settings** (Configuración)
3. En el menú lateral, busca **Pages**
4. En **Source**, selecciona **GitHub Actions**
5. Guarda los cambios

### 2. Configurar el Dominio Personalizado (Opcional)

Si quieres usar el dominio `tnovasolutions.com`:

1. En la sección **Pages**, busca **Custom domain**
2. Ingresa: `tnovasolutions.com`
3. Marca la casilla **Enforce HTTPS**
4. Guarda los cambios

### 3. Configurar DNS (Si usas dominio personalizado)

En tu proveedor de DNS, agrega estos registros:

```
Type: CNAME
Name: www
Value: va6046.github.io

Type: A
Name: @
Value: 185.199.108.153
Value: 185.199.109.153
Value: 185.199.110.153
Value: 185.199.111.153
```

### 4. Verificar el Deploy

1. Haz push de los cambios al repositorio
2. Ve a la pestaña **Actions** en GitHub
3. Verifica que el workflow se ejecute correctamente
4. Una vez completado, tu sitio estará disponible en:
   - `https://va6046.github.io/tnovasolutions` (si no usas dominio personalizado)
   - `https://tnovasolutions.com` (si configuraste el dominio personalizado)

## Solución de Problemas

### Error de Permisos
Si ves errores de permisos, asegúrate de que:
- GitHub Pages esté habilitado con **GitHub Actions** como fuente
- El workflow tenga los permisos correctos (ya configurados)

### Dominio No Funciona
Si el dominio personalizado no funciona:
- Verifica que los registros DNS estén configurados correctamente
- Espera hasta 24 horas para que los cambios DNS se propaguen
- Verifica que el archivo `CNAME` esté presente en el repositorio

## Archivos Importantes

- `.github/workflows/deploy.yml` - Workflow de deploy
- `CNAME` - Archivo para dominio personalizado
- `index.html` - Página principal
- `styles.css` - Estilos del sitio
- `script.js` - JavaScript del sitio
