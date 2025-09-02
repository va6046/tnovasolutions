# 🚀 Deploy Rápido - GitHub Pages

## ⚡ Pasos Rápidos (5 minutos)

### 1. Configurar GitHub Pages (Opcional)
El workflow ahora habilita GitHub Pages automáticamente, pero puedes configurarlo manualmente:

1. Ve a: `https://github.com/va6046/tnovasolutions/settings/pages`
2. **Source:** Selecciona **GitHub Actions**
3. **Save**

**Nota:** Si no lo configuras manualmente, el workflow lo hará automáticamente.

### 2. Crear Environment
1. Ve a: `https://github.com/va6046/tnovasolutions/settings/environments`
2. **New environment**
3. **Name:** `github-pages`
4. **Configure environment**

### 3. Hacer Deploy
```bash
git add .
git commit -m "Deploy static site to GitHub Pages"
git push origin main
```

### 4. Verificar
1. Ve a: `https://github.com/va6046/tnovasolutions/actions`
2. Espera que termine el workflow
3. Tu sitio estará en: `https://va6046.github.io/tnovasolutions`

## 🔧 Si Algo Sale Mal

### ❌ Error: "Get Pages site failed"
**Solución:** 
1. El workflow ahora habilita GitHub Pages automáticamente
2. Si persiste, crear environment `github-pages` en Settings → Environments
3. O configurar manualmente en Settings → Pages → Source: GitHub Actions

### ❌ Error: "Environment not found"
**Solución:** Crear environment `github-pages` en Settings → Environments

### ❌ Error: "Permission denied"
**Solución:** Verificar que GitHub Pages esté habilitado con GitHub Actions

### ❌ Error: "Workflow not running"
**Solución:** 
1. Ve a Actions
2. Haz clic en "Deploy to GitHub Pages"
3. "Run workflow"

### ❌ Error: "Domain not working"
**Solución:** 
1. Verificar archivo `CNAME` existe
2. Configurar DNS (ver GITHUB-PAGES-SETUP.md)

## ✅ Checklist de Deploy

- [ ] GitHub Pages habilitado con GitHub Actions
- [ ] Environment `github-pages` creado
- [ ] Archivo `CNAME` presente (si usas dominio personalizado)
- [ ] Workflow ejecutándose en Actions
- [ ] Sitio accesible en la URL

## 🎯 URLs del Sitio

- **GitHub Pages:** `https://va6046.github.io/tnovasolutions`
- **Dominio personalizado:** `https://tnovasolutions.com` (si configurado)

---

**¡Deploy en 5 minutos!** ⚡
