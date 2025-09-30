# RAP 15 - Tutorial: Herramientas de Versionamiento (GIT)

## Evidencia de producto: GA7-220501096-AA1-EV05

**Objetivo:** Conectar el equipo local con el repositorio remoto por medio de Git usando comandos básicos.

---

## 📋 Pasos Simplificados para tu Repositorio Existente

### **Paso 1: Preparar Directorio** ✅
```powershell
# Navegar al directorio del proyecto
cd "d:\Clientes\BAPE GITHUB"

# Verificar contenido actual
dir
```

### **Paso 2: Verificar Git** ✅
```powershell
# Verificar que Git está inicializado
git status

# Si no está inicializado, ejecutar:
# git init
```

### **Paso 3: Crear Archivos Requeridos** ✅
```powershell
# Crear archivo kotlin.txt con datos del usuario
echo "Nombre del usuario: IngenieroYlder" > kotlin.txt
echo "Correo electrónico: ingenieroylder@ejemplo.com" >> kotlin.txt
```

### **Paso 4: Preparar Commit**
```powershell
# Agregar cambios al staging area
git add .

# Verificar archivos agregados
git status
```

### **Paso 5: Configuración Remota (Ya configurado)**
```powershell
# Verificar repositorio remoto existente
git remote -v

# Resultado esperado:
# origin  https://github.com/IngenieroYlder/BAPE.git (fetch)
# origin  https://github.com/IngenieroYlder/BAPE.git (push)

# NOTA: Como ya tienes configurado el repositorio remoto,
# no necesitas ejecutar: git remote add origin URL
```

### **Paso 6: Push a GitHub**
```powershell
# Realizar commit
git commit -m "Añadido datos."

# Subir cambios al repositorio remoto
git push origin master
```

---

## 📚 Comandos Completos del RAP 15

### **Paso 1 - Configuración Inicial**
```bash
# 1. Crear repositorio público en GitHub con nombre "Programa-git"
# 2. Añadir repositorio remoto (YA HECHO)
git remote add github https://github.com/IngenieroYlder/BAPE.git

# 3. Mostrar repositorios remotos configurados
git remote -v
```

### **Paso 2 - Subir Cambios**
```bash
# 1. Agregar cambios del repositorio local al remoto
git push github master

# 2. Verificar en GitHub el historial de versiones
# (Acceder a la web de GitHub y revisar commits)
```

### **Paso 3 - Agregar Archivo Específico**
```bash
# 1. Crear archivo kotlin.txt con datos del usuario
cat > kotlin.txt
# (Escribir nombre y correo, luego Ctrl+C para salir)

# 2. Agregar cambios
git add .

# 3. Realizar commit con mensaje específico
git commit -m "Añadido datos."

# 4. Cargar cambios al repositorio remoto
git push origin master
```

---

## ✅ Verificación de Éxito

**Indicadores de que todo funcionó correctamente:**

1. **Terminal muestra:** "objects written" y "branch up to date"
2. **GitHub web:** Los archivos aparecen en el repositorio
3. **Historial:** Se pueden ver los commits en GitHub
4. **Estado local:** `git status` muestra "working tree clean"

---

## 📁 Estructura Final del Proyecto

```
BAPE GITHUB/
├── .gitignore          # Archivos a ignorar
├── kotlin.txt          # Datos del usuario (RAP 15)
└── RAP15-Tutorial.md   # Este tutorial
```

---

## 🔧 Comandos de Verificación

```powershell
# Verificar estado del repositorio
git status

# Ver historial de commits
git log --oneline

# Verificar conexión remota
git remote -v

# Ver diferencias si hay cambios pendientes
git diff
```

---

## 📝 Notas Importantes

- **Repositorio remoto:** Ya configurado como `origin`
- **Rama principal:** `master` (según especificaciones del RAP)
- **Archivos requeridos:** `kotlin.txt` con datos del usuario
- **Commits:** Usar mensajes descriptivos como "Añadido datos."

---

*Tutorial creado para cumplir con los requisitos del RAP 15 - Herramientas de versionamiento (GIT)*