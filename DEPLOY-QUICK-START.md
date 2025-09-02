# 🚀 Deploy Rápido - GitHub Pages

## ⚡ Pasos Rápidos (5 minutos)

### 1. Configurar GitHub Pages
1. Ve a: `https://github.com/va6046/tnovasolutions/settings/pages`
2. **Source:** Selecciona **Deploy from a branch**
3. **Branch:** Selecciona **gh-pages** (se creará automáticamente)
4. **Folder:** `/ (root)`
5. **Save**

### 2. Hacer Deploy
```bash
git add .
git commit -m "Deploy static site to GitHub Pages"
git push origin main
```

### 3. Verificar
1. Ve a: `https://github.com/va6046/tnovasolutions/actions`
2. Espera que termine el workflow
3. Tu sitio estará en: `https://va6046.github.io/tnovasolutions`

## 🔧 Si Algo Sale Mal

### ❌ Error: "Resource not accessible by integration"
**Solución:** 
1. Configurar GitHub Pages manualmente en Settings → Pages
2. Source: "Deploy from a branch"
3. Branch: "gh-pages"
4. El workflow creará la rama automáticamente

### ❌ Error: "Permission denied"
**Solución:** Verificar que GitHub Pages esté configurado correctamente

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

- [ ] GitHub Pages configurado con "Deploy from a branch"
- [ ] Rama `gh-pages` seleccionada (se crea automáticamente)
- [ ] Archivo `CNAME` presente (si usas dominio personalizado)
- [ ] Workflow ejecutándose en Actions
- [ ] Sitio accesible en la URL

## 🎯 URLs del Sitio

- **GitHub Pages:** `https://va6046.github.io/tnovasolutions`
- **Dominio personalizado:** `https://tnovasolutions.com` (si configurado)

---

**¡Deploy en 5 minutos!** ⚡
