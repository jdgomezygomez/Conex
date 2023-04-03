# Conex
Un repositorio de conexiones con una base de datos.

Es una clase PHP que conecta a una base de datos utilizando PDO, está íntimamente ligado a CodeIgniter 4, pudiendo utilizar la configuración de las conexiones de este marco, utiliza los archivos .env para recuperar información de la conexión que intenta establecer. Una vez que lo logra, siempre devuelve un puntero a la conexión, el nombre por defecto de la conexión (ya que utiliza la configuración de CodeIgniter) es 'default', y la forma de utilizarlo es:

$conex = \App\Libraries\Conex::get(string $grupo = 'default', bool $privado = false);
