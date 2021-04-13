# Páginas de erro minimalistas para Nginx

Um conjunto de páginas de erro 4xx e 5xx minimalistas personalizadas para Nginx.

Attention! This project is a simple translation of error messages into Portuguese. The original project can be found at:
https://github.com/bartosjiri/nginx-errors

## Exemplo de Página
![404 error page](https://i.imgur.com/UhkO7uP.pngg)

## Instalação

1. Navegue até o diretório de documentos padrão do Nginx:
	```
    cd /usr/share/nginx/html
    ```
2. Clone o repositório:
	```
    git clone https://github.com/cairoapcampos/nginx-errors.git
    ```

3. Adicione as páginas de erro personalizadas à configuração padrão do servidor no arquivo `/etc/nginx/sites-enabled/default`:
	```
    server {
    ...
    include /usr/share/nginx/html/nginx-errors/nginx-errors.conf
    }
    ```
4. Verifique a configuração e recarregue o Nginx:
	```
    sudo nginx -t
    sudo service nginx reload
    ```
