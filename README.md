# Buscador de Cursos Alura
Uma library composer que realiza busca de cursos da plataforma alura realizado para o curso de composer.

## Intalação
```bash
composer require pedroemanuelavelar/buscador-de-cursos
```
---
## Exemplo de uso 
```php
$client = new Client(['base_uri' => 'https://www.alura.com.br/']);

$crawler = new Crawler();

$buscador = new Buscador($client, $crawler);
$cursos = $buscador->buscar('/cursos-online-programacao/php');

foreach ($cursos as $curso) {
    echo $curso . PHP_EOL;
}
```
