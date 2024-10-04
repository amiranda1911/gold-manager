# gold-manager
Aplicação desenvolvida para o paper da disciplina de Seminário Interdisciplinar - Uniasselvi

Para executar a aplicação é necessário configurar as variáveis em config/config.php :

```php
define('APP_SEED', getenv('APP_SEED')); // valor aleatório

/* configurações do banco de dados */
define('MYSQL_HOST', getenv('MYSQL_HOST')); 
define('MYSQL_USER', getenv('MYSQL_USER'));
define('MYSQL_PASSWORD', getenv('MYSQL_PASSWORD'));
define('GOLD_APP_DATABASE', getenv('GOLD_APP_DATABASE'));
```


<host>/<controller>/<action>/<params>

```php
class <Controller>Controller extends Controller{

    public function <action> (...$params){

        $view = new View('template/view', data: array());
        $view->render();
    }
}
```

#Mapa da Aplicação

/user
lista usuarion

/user/create
cria um novo usuario

/transaction/create/{id}
cria uma nova transação para o usuario


