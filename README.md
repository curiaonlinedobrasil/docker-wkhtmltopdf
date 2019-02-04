# Docker Container - Wkhtmltopdf API
Possibilita a criação de pdfs ou imagens (png/jpg), a partir de parâmetros enviados via POST ou GET para o conteiner do serviço.

## Exemplo de formato de dados da requisição ##
```json
{
       "format": "PDF|JPG|PNG",
       "pages": [
           "<html><body><h1>Page number 1</h1></body></html>",
           "https://google.com",
           "<html><body><h1>Page number 3</h1></body></html>"
       ],
       "options": {
           "page-size"   : "A4",
           "margin-top"  : "20mm",
           "orientation" : "Portrait",
           "header-html" : "<html><head></head><body><b>This is the header</b></body></html>",
           "footer-html" : "<p>This is the footer</p>",
       }
  }
```
Para saber quais são todas as possibilidades de parâmetros no 'options', veja a documentação: https://wkhtmltopdf.org/usage/wkhtmltopdf.txt
