# Minishell

Minishell es una réplica básica de un shell de Unix. Su propósito es ejecutar comandos, implementar funcionalidades esenciales de bash y gestionar redirecciones, pipes y variables de entorno.

---

## 🧱 Estructura del Proyecto

```bash
minishell/
├── includes/       # Archivos de cabecera (.h)
├── libft/          # Biblioteca personalizada
├── Src/            # Código fuente principal
└── README.md       # Este archivo

✅ Funcionalidades

    Prompt interactivo

    Ejecución de comandos con argumentos

    Soporte para múltiples pipes (|)

    Redirecciones:

        Entrada <

        Salida >, >>

        Heredoc <<

    Variables de entorno ($VAR)

    Built-ins implementados:

        cd, echo, env, exit, export, pwd, unset

    Manejo de señales (Ctrl+C, Ctrl+\, Ctrl+D)

    Gestión de errores

    Códigos de retorno correctos ($?)

⚙️ Requisitos

    Sistema Linux/Unix

    gcc y make

    Librería readline

Instalación en sistemas Debian/Ubuntu:

sudo apt-get install libreadline-dev

🔨 Compilación

make

Se genera un binario llamado minishell.
▶️ Uso

./minishell

Ejemplos de comandos soportados:

echo hola mundo
ls -l | grep minishell
cat << EOF
export VAR=42 && echo $VAR

🧪 Testing

Prueba comandos básicos, combinaciones con redirecciones y pipes, y variables de entorno.
