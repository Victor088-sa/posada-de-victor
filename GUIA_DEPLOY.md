# 📋 INSTRUCCIONES PARA SUBIR TU SITIO A NETLIFY

## ✅ Tu Proyecto Está Listo

Tu proyecto tiene esta estructura final:

```
POSADA DE VICTOR/
├── index.html              ⭐ Archivo principal
├── README.md               📖 Documentación
├── .gitignore              🔒 Archivo de Git
├── netlify.toml            ⚙️ Configuración Netlify
└── assets/
    ├── images/             📸 7 fotos (webp y jpeg)
    └── videos/             🎬 video-1.mp4
```

---

## 🚀 PASO 1: Instalar Git (Si no lo tienes)

**Windows:**
1. Descarga: https://git-scm.com/download/win
2. Instala con los valores por defecto
3. Abre PowerShell y verifica: `git --version`

---

## 📤 PASO 2: Subir a GitHub

### 2.1 Crear Repositorio en GitHub

1. Ve a https://github.com (crea cuenta si no tienes)
2. Click en "New repository"
3. Nombre: `posada-de-victor`
4. Descripción: "Sitio web de la Posada de Víctor"
5. Click "Create repository"

### 2.2 Conectar tu Carpeta Local con Git

Abre PowerShell en la carpeta `POSADA DE VICTOR` y ejecuta:

```powershell
# Inicializar Git
git init

# Agregar todos los archivos
git add .

# Crear primer commit
git commit -m "Sitio inicial de Posada de Víctor"

# Agregar el repositorio remoto (REEMPLAZA tu_usuario)
git remote add origin https://github.com/tu_usuario/posada-de-victor.git

# Subir los cambios
git branch -M main
git push -u origin main
```

✅ ¡Listo! Tu código está en GitHub

---

## 🌐 PASO 3: Desplegar en Netlify

### 3.1 Conectar GitHub a Netlify

1. Ve a https://netlify.com
2. Haz click en "Sign up"
3. Elige "Sign up with GitHub" (es más fácil)
4. Autoriza a Netlify
5. Aparecerá "Create a new site"

### 3.2 Seleccionar Repositorio

1. Click en "Connect to Git"
2. Selecciona "GitHub"
3. Busca y selecciona: `posada-de-victor`
4. Click "Deploy site"

✅ **¡TU SITIO ESTÁ EN LÍNEA!** Netlify te dará una URL como:
```
https://random-name-123.netlify.app
```

---

## 🎯 PASO 4: Conectar tu Dominio Personalizado

### 4.1 Registrar Dominio en Namecheap

1. Ve a https://namecheap.com
2. Busca: `posadadevictor.com` (o variantes)
3. Compra por ~$10 USD/año
4. Completa el registro

### 4.2 Conectar Dominio a Netlify

**En Netlify:**
1. Ve a "Domain settings"
2. Click "Add custom domain"
3. Escribe: `posadadevictor.com`
4. Netlify te dirá que apuntes los servidores DNS

**En Namecheap:**
1. Vuelve a tu panel de Namecheap
2. Ve a "Domain List" → tu dominio
3. Click "Manage"
4. Va a "Nameservers"
5. Selecciona "Custom DNS"
6. Agrega los nameservers de Netlify (te los dice cuando agregas dominio)
7. Guarda cambios

⏱️ **Espera 24 horas** para que se propague el DNS

✅ **¡Ahora tu sitio está en `posadadevictor.com`!**

---

## 🔒 HTTPS/SSL (Automático)

Netlify configura SSL automáticamente. Tu sitio será `https://posadadevictor.com` 🔐

---

## 📝 ACTUALIZACIONES FUTURAS

Cada vez que hagas cambios:

```powershell
# En tu carpeta del proyecto
git add .
git commit -m "Descripción del cambio"
git push
```

Netlify se actualiza **automáticamente** en 1 minuto ⚡

---

## 🆘 PROBLEMAS COMUNES

### "No funciona el sitio después de subir"
- Verifica que `index.html` esté en la **raíz**
- Verifica que `assets/` esté en el mismo nivel que `index.html`
- Comprueba las rutas: `assets/images/foto.webp` ✅ (NO `img/foto.webp`)

### "Las imágenes no cargan"
- Comprueba que existan en `assets/images/`
- Asegúrate que las rutas sean relativas (sin `/` al inicio)

### "¿Cuánto cuesta Netlify?"
- **Hosting:** GRATIS ✅
- **Dominio:** ~$10/año en Namecheap
- **Total:** $10/año

---

## 📊 RESUMEN DE COSTOS ANUALES

| Concepto | Costo |
|----------|-------|
| Dominio (.com) | $10 USD |
| Hosting (Netlify) | GRATIS |
| **TOTAL** | **$10 USD** |

---

## 🎉 ¡LISTO!

Tu sitio de Posada de Víctor estará en:
```
https://posadadevictor.com
```

Con:
- ✅ Dominio profesional
- ✅ HTTPS/SSL gratis
- ✅ Actualizaciones automáticas
- ✅ Servidor ultrarrápido
- ✅ Análiticas incluidas
- ✅ 0 configuración backend

---

**¿Necesitas ayuda en algún paso?** ¡Pregúntame!
